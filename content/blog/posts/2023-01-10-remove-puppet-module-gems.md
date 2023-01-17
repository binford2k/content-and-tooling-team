---
title: "Removing puppet-modules-gems"
date: 2023-01-10
author: "David Swan"
github_repo: "" # Disable the edit commands
---

## What are `puppet-module-gems` and why are they now considered harmful?
Okay, that might be a bit of a melodramatic take on the situation, but the `puppet-module-gems` really did serve a useful purpose at one point. Let's go back over why it exists and what's changed in the meantime.

We'll start with Bundler--a local environment manager for Ruby projects.
It runs a Ruby project with all of its required dependencies in a sandbox, meaning that you don't need to install gems globally.
This is great for repeatability and means that each project can have the specific gem versions it requires without interfering with other projects that might need different versions.

This worked great for Puppet back in the good old days when things were simple.
All the gems Puppet used were specified in the `Gemfile` and Bundler environments just worked.
But then the Ruby ecosystem evolved and gems started taking advantage of new functionality.
Version 1.2 of a gem might run on Ruby 1.8, but an upgrade to version 1.4 was required to use Ruby 2.0 and then Ruby 2.5 needed yet another version.
This got to be rather complex, and worse *Bundler couldn't resolve these dependencies properly!* We had to [do it ourselves](https://github.com/puppetlabs/puppetlabs-stdlib/blob/4b15c970f5ac6bc683cfde32d782f51a63bee867/Gemfile#L29-L34), making the `Gemfiles` brittle and harder to read and maintain.

CI was breaking, module authors were struggling to test on multiple platforms, users were having a hard time validating updates.
Clearly we needed a solution, and the `puppet-module-gems` were the answer.
We created meta-gems for each Ruby version we supported and specified the proper dependencies in these gems.
Then the `Gemfile` would conditionally depend on the properly versioned meta-gem based on the version of Ruby running.

This worked reasonably well, but had its challenges.
The dependencies were opaque and the extra level of abstraction meant that looking at the `Gemfile` didn't really tell you much about what gems would be installed or used.
Worse, we had to manually resolve and specify all the dependencies for every Ruby version, and keeping up with those turned out to be easier said than done.
We often fell behind and our more adventurous users would regularly [remind us of that](https://tickets.puppetlabs.com/browse/MODULES-11161).
The situation certainly wasn't ideal, but it was a workable compromise.

Until Bundler got smarter, learned how to resolve Ruby version dependencies, and made this workaround no longer necessary.

## What's Changing
With these Bundler updates, we no longer require such tight control over dependencies, since Bundler will do the right thing and resolve them properly, taking gems' supported Ruby versions into account. We have decided to stop maintaining the `puppet-module-gems` and instead move fully to managing our gem dependencies with the PDK templates. This will be easier to maintain in the long term and will better allow downstream users to modify according to their own needs.

This is especially relevant now as it means that the `puppet-modules-gems` have not been updated to account for Ruby 3, which the upcoming Puppet 8 release will release with. **This means that any module that has not yet converted to the new format will be not be testable on Puppet 8**.

## What You Need To Do
If you maintain your own Puppet modules, the rest of this post is for you.
If you only *use* modules from the Forge, then no action is necessary on your part, other than to file bug reports with a link to this blog post if you notice modules which should be updated.

Thankfully, the solution to adopting the new standard is relatively simple, at least for those who are using the PDK and the default templates. We've already made the updates for you and you'll just need to update your module with these changes. This will replace `puppet-module-gems` in the `Gemfile` with the actual dependencies that the meta-gem represented.

```
$ pdk update
```

An example of the changes this update includes can be seen on many of our modules, with one example shown [here](https://github.com/puppetlabs/puppetlabs-apache/pull/2324).

In the event that you are not using the default PDK templates then you will need to update each `Gemfile` yourself. Look at the config default values [here](https://github.com/puppetlabs/pdk-templates/blob/dd87389c8e88f312861e57cea2d3d4ba52af2bd7/config_defaults.yml#L556) and copy what you need into your own template repository, updating them according to your own needs.

If you are not using the PDK at all, you can find an example of a current `Gemfile` below, which you can copy and modify as you need. Tracking the default versions listed under the `Gemfile` key in [config_defaults.yml](https://github.com/puppetlabs/pdk-templates/blob/main/config_defaults.yml) will help you keep these versions correct as you update over time.

```
group :development do
# These where already set in pdk templates and so may not be relevant to you
  gem "json", '~> 2.0',                                require: false
  gem "voxpupuli-puppet-lint-plugins", '~> 3.0',       require: false

# The main group of rules we are adding
  gem "facterdb", '~> 1.18',                           require: false
  gem "metadata-json-lint", '>= 2.0.2', '< 4.0.0',     require: false
  gem "puppetlabs_spec_helper", '>= 2.9.0', '< 4.0.0', require: false
  gem "rspec-puppet-facts", '>= 1.10.0', '< 3.0.0',    require: false
  gem "codecov", '~> 0.2',                             require: false
  gem "dependency_checker", '~> 0.2',                  require: false
  gem "parallel_tests", '~> 3.4',                      require: false
  gem "pry", '~> 0.10',                                require: false
  gem "simplecov-console", '~> 0.5',                   require: false
  gem "puppet-debugger", '~> 1.0',                     require: false

## We pin these in order to keep the style rules static
  gem "rubocop", '= 1.6.1',                            require: false
  gem "rubocop-performance", '= 1.9.1',                require: false
  gem "rubocop-rspec", '= 2.0.1',                      require: false
  gem "rb-readline", '= 0.5.5',                        require: false, platforms: [:mswin, :mingw, :x64_mingw]

# Added locally and used by us as part of the release process, may not be relevant to you
  gem "github_changelog_generator",                    require: false
end

group :system_tests do
  gem "puppet_litmus", '< 1.0.0', require: false, platforms: [:ruby]
  gem "serverspec", '~> 2.41',    require: false
end
```

## Conclusions
Since we are not un-publishing the existing `puppet-module-gems` meta-gems, we don't expect many people to be impacted by this change.
Many module authors won't even notice it, as they'll `pdk update` their modules naturally at some point and inherit the updates before it becomes critical for them.
What this does mean, though, is that you should get more used to running `pdk update` regularly as this is the standard way in which updated dependencies and support for new Ruby versions will be delivered.

Good luck, and happy Puppeting!






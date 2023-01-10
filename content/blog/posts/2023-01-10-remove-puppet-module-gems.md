---
title: "Removing puppet-modules-gems"
date: 2023-01-10
author: "David Swan"
github_repo: "" # Disable the edit commands
---

## Introduction
With the updates made to bundler we no longer require as tight a control of our gem files as previously had been necessary. This has led us to make the decision to stop maintaining the `puppet-module-gems` and instead move fully to managing our gems with the PDK templates, as we fee that it will be easier to maintain in the long term and will better allow downstream users to modify according to their own needs.

This is especially relevant now as it means that the `puppet-modules-gems` have not been updated to account for Ruby 3, which the upcoming Puppet 9 release will release with, meaning that any module that has not yet converted to the new format will be unable to run on Puppet 9.

## What To Do
Thankfully, the solution to this is relatively simple, at least for those who are using our PDK templates. The only thing that you will need to do is run an update against the main branch of the templates and the changes made to it will be consumed, replacing `puppet-module-gems` in the Gemfile with the multiple seperate gems that it consisted off. An example of this can be seen on many of our modules, with one example shown [here](https://github.com/puppetlabs/puppetlabs-apache/pull/2324).

In the event that you are not using the pdk template then you will need to update your Gemfiles in another way, however this to should not be much of an issue. If you are using the PDK but with your own version of the template, simply look at the config default values [here](https://github.com/puppetlabs/pdk-templates/blob/main/config_defaults.yml#L556) and copy what you need into your own code, updating them according to your own needs.

If you are not using the PDK at all, you can find an example of a current Gemfile below, simply copy and modify as you need:
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

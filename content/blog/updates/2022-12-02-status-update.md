---
author: "GSPatton"
categories:
  - updates
date: "2022-12-02"
blog_tags: null
title: "2022-12-02: Content & Tooling Team Status Update"
---
# It's beginning to look a lot like Christmas
![Merry Christmas](https://media.giphy.com/media/z1qogLd15kVMfhKEMu/giphy.gif)

Happy Friday eveyone! And happy holidays! It's definitely beginning to look a lot like Christmas in Belfast. We even had a Christmas jumper and office decoration day on Wednesday to welcome in the festive season.

# Our finest gifts we bring pa rum pum pum pum...

## PDK User Survey
In order for us to understand how to build a better PDK, [I][Gavin] have created a [user survey](https://forms.office.com/r/TiFvqtEU8Z). We'd love to get a response from you! The submission deadline is the 16th of December and following this we will analyse the data so that we are ready to start planning the next steps for PDK in the new year! Exciting times!

## PDK Deep Dive
On the topic of PDK, [Craig][Craig] has bravely ventured into the depths of PDK. We pray he returns safe and sound.

## Codebase Hardening
We have officially finished hardening our codebase. The team have put in a massive effort over the past few months to make our modules more secure. Big shout out to [Lukas][Lukas], [Craig][Craig] and [David][David].

## Puppet Lint Unsafe Interpolations Plugin
[I][Gavin] have created an MVP [gem](https://rubygems.org/gems/puppet-lint-check_unsafe_interpolations) for the puppet-lint unsafe interpolation plugin. We are currently testing this out and would be grateful for any feedback.

## In other news...
[Lukas][Lukas] has been fixing some bugs in the Kubernetes module and [David][David] has officially finished removing puppet-module-gems.

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`pdk-templates#484`][pdk-templates-pr-484]: "voxpupuli-puppet-lint-plugins: Pull in 3.1 or newer", thanks to [bastelfreak][bastelfreak]

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-docker`][puppetlabs-docker] (`6.0.1`)
- [`puppetlabs-java`][puppetlabs-java] (`9.0.1`)

  [puppetlabs-docker]: https://github.com/puppetlabs/puppetlabs-docker
  [puppetlabs-java]: https://github.com/puppetlabs/puppetlabs-java
  [pdk-templates-pr-484]: https://github.com/puppetlabs/pdk-templates/pull/484
  [bastelfreak]: https://github.com/bastelfreak
  [Craig]: https://github.com/chelnak
  [David]: https://github.com/david22swan
  [Lukas]: https://github.com/LukasAud
  [Gavin]: https://github.com/GSPatton

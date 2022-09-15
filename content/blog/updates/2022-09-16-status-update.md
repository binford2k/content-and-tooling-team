---
author: "david22swan"
categories:
  - updates
date: "2022-09-16"
blog_tags: null
title: "2022-09-16: Content & Tooling Team Status Update"
---

## Another week gone by

Another week has passed and we are here again to give you an update on what had been going on.

## DSC

Work has been continued on the DSC base provider by our own [Craig][chelnak] with a bug preventing the honoring of metaparameters being fixed. This shoudl go out in a rwby-pwsh release some time next week.

## Clarification of Support

Many of our modules have drifted over the years, making the support OS section of our modules inaccurate at times. In order to resolve this both [Jordan][Jordan] and [Gavin][Gavin] have been working hard, going through each and every one of our supported modules and ensuring that the support that we claim is in line with what we intend to provide.

## Ruby 3 Support

It has been an unfortunate fact that our ruby support has started to lag behind in recent times, with Ruby 3 having done unsupported by our [puppet-module-gems][puppet-module-gems].
This is something that we are currently aiming to resolve with [I myself][David] having begun an investigation into adding support for Ruby 3 and 3.1 and the way in which we can ensure this does not occur again in the future.

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`puppetlabs-accounts#417`][puppetlabs-accounts-pr-417]: "Removing support for Centos 8", thanks to [jordanbreenpuppet][jordanbreenpuppet] and the following people who helped get it over the line ([kenyon][kenyon])
- [`puppetlabs-acl#265`][puppetlabs-acl-pr-265]: "Removing unsupported windows versions", thanks to [jordanbreenpuppet][jordanbreenpuppet]
- [`puppetlabs-apache#2314`][puppetlabs-apache-pr-2314]: "(MAINT) Removing support for CentOS 8", thanks to [jordanbreenpuppet][jordanbreenpuppet]
- [`puppetlabs-apache#2301`][puppetlabs-apache-pr-2301]: "Allow RewriteInherit with empty rewrites", thanks to [martin-koerner][martin-koerner]
- [`puppetlabs-docker#856`][puppetlabs-docker-pr-856]: "Update supported Ubuntu versions in README", thanks to [nikzeyn][nikzeyn]
- [`puppetlabs-vcsrepo#566`][puppetlabs-vcsrepo-pr-566]: "Only remove safe_directory, if it exists", thanks to [KoenDierckx][KoenDierckx] and the following people who helped get it over the line ([elfranne][elfranne])

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-vcsrepo`][puppetlabs-vcsrepo] (`5.3.0`)
- [`puppetlabs-apache`][puppetlabs-apache] (`8.2.0`)
- [`puppetlabs-tomcat`][puppetlabs-tomcat] (`6.3.0`)

  [puppetlabs-vcsrepo]: https://github.com/puppetlabs/puppetlabs-vcsrepo
  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-tomcat]: https://github.com/puppetlabs/puppetlabs-tomcat
  [puppetlabs-accounts-pr-417]: https://github.com/puppetlabs/puppetlabs-accounts/pull/417
  [jordanbreenpuppet]: https://github.com/jordanbreenpuppet
  [kenyon]: https://github.com/kenyon
  [puppetlabs-acl-pr-265]: https://github.com/puppetlabs/puppetlabs-acl/pull/265
  [puppetlabs-apache-pr-2314]: https://github.com/puppetlabs/puppetlabs-apache/pull/2314
  [puppetlabs-apache-pr-2301]: https://github.com/puppetlabs/puppetlabs-apache/pull/2301
  [martin-koerner]: https://github.com/martin-koerner
  [puppetlabs-docker-pr-856]: https://github.com/puppetlabs/puppetlabs-docker/pull/856
  [nikzeyn]: https://github.com/nikzeyn
  [puppetlabs-vcsrepo-pr-566]: https://github.com/puppetlabs/puppetlabs-vcsrepo/pull/566
  [KoenDierckx]: https://github.com/KoenDierckx
  [elfranne]: https://github.com/elfranne
  [Craig]: https://github.com/chelnak
  [Gavin]: https://github.com/GSPatton
  [Jordan]: https://github.com/jordanbreenpuppet
  [David]: https://github.com/david22swan
  [puppet-module-gems]: https://github.com/puppetlabs/puppet-module-gems

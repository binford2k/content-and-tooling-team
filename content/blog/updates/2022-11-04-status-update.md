---
author: "LukasAud"
categories:
  - updates
date: "2022-11-04"
blog_tags: null
title: "2022-11-04: Content & Tooling Team Status Update"
---

## First Friday of November

As we leave October and start packing our halloween decorations, some of us can already hear the classic christmas songs playing in the distance. 
Almost no time left before we start hearing "All I want for Christmas is you" in every single store everywhere.

## Community and releases

As usual, we had a busy community day, happily merging up to 12 community Pull Requests. Big thanks to everyone for your contributions.
We also had the chance to cut a release for Apache and a major one for Chocolatey, where we addressed some incompatibility issues.

## Steady work
Most of our team is still working on the background to complete some of our highest priority projects.

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`puppetlabs-apache#2340`][puppetlabs-apache-pr-2340]: "Extract acceptance node setup to a separate file", thanks to [ekohl][ekohl]
- [`puppetlabs-apache#2333`][puppetlabs-apache-pr-2333]: "Fix RedHat + PHP 8 libphp file", thanks to [polatsinan][polatsinan]
- [`puppetlabs-apt#1069`][puppetlabs-apt-pr-1069]: "Do not remove PPA sources.list.d files if purge is enabled", thanks to [Programie][Programie]
- [`puppetlabs-java_ks#412`][puppetlabs-java_ks-pr-412]: "reversed insync set comparison", thanks to [rstuart-indue][rstuart-indue]
- [`puppetlabs-kubernetes#577`][puppetlabs-kubernetes-pr-577]: "Add RedHat family as supported OS (#563)", thanks to [deric][deric]
- [`puppetlabs-kubernetes#576`][puppetlabs-kubernetes-pr-576]: "Switch containerd grpc socket to URI", thanks to [towo][towo]
- [`puppetlabs-mysql#1505`][puppetlabs-mysql-pr-1505]: "mysql::db sql parameter support filenames with multiple dots", thanks to [skn-bvdh][skn-bvdh] and the following people who helped get it over the line ([leemachine][leemachine])
- [`puppetlabs-postgresql#1374`][puppetlabs-postgresql-pr-1374]: "Rewrite dependency installation using native Puppet", thanks to [ekohl][ekohl]
- [`puppetlabs-tomcat#501`][puppetlabs-tomcat-pr-501]: "Exclude name in resources", thanks to [kobybr][kobybr]
- [`puppetlabs-vcsrepo#576`][puppetlabs-vcsrepo-pr-576]: "support per-repo HTTP proxy for the git provider", thanks to [bugfood][bugfood]
- [`puppetlabs-vcsrepo#575`][puppetlabs-vcsrepo-pr-575]: "fix repeated acceptance tests on the same container", thanks to [bugfood][bugfood]
- [`facterdb#257`][facterdb-pr-257]: "Fix Red Hat facts on version 4.2", thanks to [anders-larsson][anders-larsson] and the following people who helped get it over the line ([bastelfreak][bastelfreak], [ekohl][ekohl])

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-apache`][puppetlabs-apache] (`8.3.0`)
- [`puppetlabs-chocolatey`][puppetlabs-chocolatey] (`7.0.0`)

  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-chocolatey]: https://github.com/puppetlabs/puppetlabs-chocolatey
  [puppetlabs-apache-pr-2340]: https://github.com/puppetlabs/puppetlabs-apache/pull/2340
  [ekohl]: https://github.com/ekohl
  [puppetlabs-apache-pr-2333]: https://github.com/puppetlabs/puppetlabs-apache/pull/2333
  [polatsinan]: https://github.com/polatsinan
  [puppetlabs-apt-pr-1069]: https://github.com/puppetlabs/puppetlabs-apt/pull/1069
  [Programie]: https://github.com/Programie
  [puppetlabs-java_ks-pr-412]: https://github.com/puppetlabs/puppetlabs-java_ks/pull/412
  [rstuart-indue]: https://github.com/rstuart-indue
  [puppetlabs-kubernetes-pr-577]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/577
  [deric]: https://github.com/deric
  [puppetlabs-kubernetes-pr-576]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/576
  [towo]: https://github.com/towo
  [puppetlabs-mysql-pr-1505]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1505
  [skn-bvdh]: https://github.com/skn-bvdh
  [leemachine]: https://github.com/leemachine
  [puppetlabs-postgresql-pr-1374]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1374
  [puppetlabs-tomcat-pr-501]: https://github.com/puppetlabs/puppetlabs-tomcat/pull/501
  [kobybr]: https://github.com/kobybr
  [puppetlabs-vcsrepo-pr-576]: https://github.com/puppetlabs/puppetlabs-vcsrepo/pull/576
  [bugfood]: https://github.com/bugfood
  [puppetlabs-vcsrepo-pr-575]: https://github.com/puppetlabs/puppetlabs-vcsrepo/pull/575
  [facterdb-pr-257]: https://github.com/voxpupuli/facterdb/pull/257
  [anders-larsson]: https://github.com/anders-larsson
  [bastelfreak]: https://github.com/bastelfreak

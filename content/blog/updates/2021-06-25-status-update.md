---
author: '@peculiarism'
categories:
- team
- status
date: "2021-06-25T00:00:00Z"
blog_tags:
- pct
- pdk
- concat
- apache
- firewall
- haproxy
- mysql
title: '2021-06-25: IAC & DevX Team Status Update'
---

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`puppetlabs-apache#2158`][puppetlabs-apache-pr-2158]: "Update the default version of Apache for Amazon Linux 2", thanks to [turnopil][turnopil] and the following people who helped get it over the line ([NapoSky][NapoSky], [ekohl][ekohl])
- [`puppetlabs-apache#2154`][puppetlabs-apache-pr-2154]: "Only warn about servername logging if relevant", thanks to [ekohl][ekohl]
- [`puppetlabs-docker#755`][puppetlabs-docker-pr-755]: "Add syslog_facility parameter to docker::run", thanks to [waipeng][waipeng]
- [`puppetlabs-haproxy#486`][puppetlabs-haproxy-pr-486]: "Fix haproxy_version fact for versions >= 2.4.0", thanks to [bp85][bp85]
- [`puppetlabs-mysql#1403`][puppetlabs-mysql-pr-1403]: "Fix broken link and style in documentation", thanks to [ghoneycutt][ghoneycutt]
- [`puppetlabs-mysql#1400`][puppetlabs-mysql-pr-1400]: "Use Puppet-Datatype Sensitive", thanks to [cocker-cc][cocker-cc]
- [`facterdb#172`][facterdb-pr-172]: "cleanup documentation + migrate CI+release process from travis to github actions", thanks to [bastelfreak][bastelfreak]
- [`facterdb#170`][facterdb-pr-170]: "Add Facter 4 facts for Debian 10/CentOS 7", thanks to [genebean][genebean] and the following people who helped get it over the line ([bastelfreak][bastelfreak])
- [`facterdb#169`][facterdb-pr-169]: "Add Sparc Solaris 11 Facter 4 facts", thanks to [genebean][genebean]
- [`puppet-resource_api#289`][puppet-resource_api-pr-289]: "Only ship needed files", thanks to [ekohl][ekohl] and the following people who helped get it over the line ([puppetlabs-jenkins][puppetlabs-jenkins])

Check [all the ways to reach us](/blog/updates/2021-01-20-reaching-out.md) if you want to directly contact us about anything module related.

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-concat`][puppetlabs-concat] (`7.0.2`)
- [`puppetlabs-apache`][puppetlabs-apache] (`6.3.0`)
- [`puppetlabs-firewall`][puppetlabs-firewall] (`3.0.1`)
- [`puppetlabs-haproxy`][puppetlabs-haproxy] (`6.0.2`)
- [`puppetlabs-mysql`][puppetlabs-mysql] (`11.0.3`)

  [puppetlabs-concat]: https://github.com/puppetlabs/puppetlabs-concat
  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-firewall]: http://github.com/puppetlabs/puppetlabs-firewall
  [puppetlabs-haproxy]: https://github.com/puppetlabs/puppetlabs-haproxy
  [puppetlabs-mysql]: http://github.com/puppetlabs/puppetlabs-mysql
  [puppetlabs-apache-pr-2158]: https://github.com/puppetlabs/puppetlabs-apache/pull/2158
  [turnopil]: https://github.com/turnopil
  [NapoSky]: https://github.com/NapoSky
  [ekohl]: https://github.com/ekohl
  [puppetlabs-apache-pr-2154]: https://github.com/puppetlabs/puppetlabs-apache/pull/2154
  [puppetlabs-docker-pr-755]: https://github.com/puppetlabs/puppetlabs-docker/pull/755
  [waipeng]: https://github.com/waipeng
  [puppetlabs-haproxy-pr-486]: https://github.com/puppetlabs/puppetlabs-haproxy/pull/486
  [bp85]: https://github.com/bp85
  [puppetlabs-mysql-pr-1403]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1403
  [ghoneycutt]: https://github.com/ghoneycutt
  [puppetlabs-mysql-pr-1400]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1400
  [cocker-cc]: https://github.com/cocker-cc
  [facterdb-pr-172]: https://github.com/voxpupuli/facterdb/pull/172
  [bastelfreak]: https://github.com/bastelfreak
  [facterdb-pr-170]: https://github.com/voxpupuli/facterdb/pull/170
  [genebean]: https://github.com/genebean
  [facterdb-pr-169]: https://github.com/voxpupuli/facterdb/pull/169
  [puppet-resource_api-pr-289]: https://github.com/puppetlabs/puppet-resource_api/pull/289
  [puppetlabs-jenkins]: https://github.com/puppetlabs-jenkins

The team has been very focused this week on supporting some of Puppet's internal teams with IAC tooling, big shout out to [Danny][Danny] for jumping in to help the support team, and [Sheena][Sheena] stepping in to onboard the PIE team with Litmus capabilities. Inclusive of this work the team managed to process **36** issues/tickets/PRs across both tooling and supported modules, go team!

## DevX Team Update

It's been a busy week on the DevX team!
We're delighted to announce the release of PDK version `2.1.1`.
This release resolves an issue in which [child processes were unable to spawn](https://puppet.com/docs/pdk/2.x/release_notes_pdk.html#resolved-issue-with-access-denied-error-on-win-github-actions) on some Windows systems.
Check out the [release notes](https://puppet.com/docs/pdk/2.x/release_notes_pdk.html) for a full list of enhancements and fixes that have gone in to `2.1.1`.
We also have a new release of the [PCT tool]( /blog/updates/2021-06-04-pct-early-release.md). Version `0.2.0` can be installed over the top of `0.1.0` using these [installation instructions](https://github.com/puppetlabs/pct#installing).
Check out the [the `0.2.0` release page](https://github.com/puppetlabs/pct/releases/tag/0.2.0) for full details of what's included.

## Community shout out

The team wanted to give a big shoutout to [cocker-cc][cocker-cc] and their work on implementing the Puppet `Sensitive Datatype` across some of our supported modules like [puppetlabs-haproxy](https://github.com/puppetlabs/puppetlabs-haproxy/pull/487), [puppetlabs-mysql](https://github.com/puppetlabs/puppetlabs-mysql/pull/1400) and [puppetlabs-postgresql](https://github.com/puppetlabs/puppetlabs-postgresql/pull/1279).

<!-- check https://tickets.puppetlabs.com/secure/RapidBoard.jspa?rapidView=1176&quickFilter=8745 for other tickets closed out this week that should be mentioned here -->

  [Adrian]:             https://github.com/adrianiurca
  [Ben]:                https://github.com/binford2k
  [Ciaran]:             https://github.com/sanfrancrisko
  [Daiana]:             https://github.com/daianamezdrea
  [Danny]:              https://github.com/carabasdaniel
  [DavidArmstrong]:     https://github.com/da-ar
  [DavidSchmitt]:       https://github.com/DavidS
  [DavidSwan]:          https://github.com/david22swan
  [Disha]:              https://github.com/Disha-maker
  [James]:              https://github.com/jpogran
  [Lore]:               https://github.com/lionce
  [Michael]:            https://github.com/michaeltlombardi
  [Paula]:              https://github.com/pmcmaw
  [Sheena]:             https://github.com/sheenaajay
  [Supported Modules]:  https://puppetlabs.github.io/iac/modules/
  [Tools]:              https://puppetlabs.github.io/iac/tools/

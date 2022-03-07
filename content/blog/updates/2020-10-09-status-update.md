---
author: daianamezdrea
categories:
- team
- status
date: "2020-10-09T00:00:00Z"
blog_tags:
- concat
- apache
- exec
- firewall
- stdlib
- puppet_intern
- dsc
title: '2020-10-09: IAC Team Status Update'
---

## Community Contributions

We had a busy week and the community was very active so we'd like to thank the following people in the Puppet Community for their contributions over this past week:

 Thanks to [jcpunk][jcpunk] for the folowing PRs where he resolves `puppet-lint` and `yamllint` warnings across the following repos: 
- [`puppetlabs-apache#2066`][puppetlabs-apache-pr-2066], thanks also to [igalic][igalic], who helped get it over the line.
- [`puppetlabs-mysql#1327`][puppetlabs-mysql-pr-1327]
- [`puppetlabs-inifile#414`][puppetlabs-inifile-pr-414]
- [`puppetlabs-motd#333`][puppetlabs-motd-pr-333]
- [`puppetlabs-postgresql#1191`][puppetlabs-postgresql-pr-1191]
- [`puppetlabs-firewall#945`][puppetlabs-firewall-pr-945]: Thanks to [pellisesol][pellisesol] for ading carp protocol to :proto property.
- [`puppetlabs-stdlib#1133`][puppetlabs-stdlib-pr-1133]: Thanks to [smortex][smortex] for his fix from CHANGELOG.md.
- [`puppetlabs-concat#661`][puppetlabs-concat-pr-661]: Thanks to [seanmil][seanmil] who treats the case when no concat_fragment resources are specified.

## New Module / Gem Releases

The following modules were released this week:
- [`puppetlabs-apache`][puppetlabs-apache] (`5.6.0`)
- [`puppetlabs-firewall`][puppetlabs-firewall] (`2.6.0`)
- [`puppetlabs-exec`][puppetlabs-exec] (`0.8.0`)

## Life of an intern at Puppet

 [Disha][disha-maker] continues her journey at Puppet and [here](https://puppetlabs.github.io/iac/docs/life_of_intern) you can find the last updates of ** Life of an intern at Puppet ** .

## DSC

With the first customers starting to use the [wonderful new DSC modules](https://puppetlabs.github.io/iac/news/roadmap/2020/09/21/dsc-release.html) we encountered some hurdles when directly upgrading from old DSC management options. While we're working on a complete fix, we recommend for now to start with removing old DSC modules completely before rolling out the new. For any DSC issues, you can always find us [here](https://github.com/puppetlabs/puppetlabs-dsc) ready to help!

## CI Improvements

Work continues on a solution for public on-demand acceptance tests for modules. This week saw us finishing up a fully automated deployment solution for all the involved cloud components, some light testing, and tightening up of code. If nothing goes horribly wrong, we'll be able to share more details and a sneak-peak of the final results in the next two weeks.

If you want to know about the project in person, check out the [Puppet Hacktoberfest Hackathon](https://puppet.com/blog/hacktoberfest-2020/) on 20 October, 2020 (GMT and PST).

## Wrap-up

That's it for this weeks update, have a great weekend everyone! 

  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-firewall]: http://github.com/puppetlabs/puppetlabs-firewall
  [puppetlabs-exec]: https://github.com/puppetlabs/puppetlabs-exec
  [puppetlabs-apache-pr-2066]: https://github.com/puppetlabs/puppetlabs-apache/pull/2066
  [jcpunk]: https://github.com/jcpunk
  [igalic]: https://github.com/igalic
  [disha-maker]: https://github.com/disha-maker
  [seanmil]: https://github.com/seanmil
  [puppetlabs-firewall-pr-945]: https://github.com/puppetlabs/puppetlabs-firewall/pull/945
  [pellisesol]: https://github.com/pellisesol
  [puppetlabs-inifile-pr-414]: https://github.com/puppetlabs/puppetlabs-inifile/pull/414
  [puppetlabs-motd-pr-333]: https://github.com/puppetlabs/puppetlabs-motd/pull/333
  [puppetlabs-mysql-pr-1327]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1327
  [puppetlabs-postgresql-pr-1191]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1191
  [puppetlabs-stdlib-pr-1133]: https://github.com/puppetlabs/puppetlabs-stdlib/pull/1133
  [puppetlabs-concat-pr-661]: https://github.com/puppetlabs/puppetlabs-concat/pull/661
  [smortex]: https://github.com/smortex

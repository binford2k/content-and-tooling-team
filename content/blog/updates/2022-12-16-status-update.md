---
author: "LukasAud"
categories:
  - updates
date: "2022-12-16"
blog_tags: null
title: "2022-12-16: Content & Tooling Team Status Update"
---

## One week left 'till holidays
Finally, Christmas and our Winter Holidays are already around the corner, with only one more week to go. With the prospect of a nice winter break with our families in our minds, we have been busy working to ensure that
we are ready for what's to come next year.

## Kubernetes
Our Kubernetes module experienced a setback recently as we tried to implement some a codebase hardening update in it that did not work as intended. However, thanks to [chelnak][chelnak] and the community's involvement, we
are happy to announce that Kubernetes is back in a healthy state and freshly released in the forge. We would like to give a big shout out to [deric][deric] and his amazing work for helping us get this release out of the door.

## Module maintenance
Some of our modules have been sitting idle for a bit too long and, thus, some of their code has fallen behind. That's why we are working on some module maintenance to update the syntax and datatypes of all modules and
ensure that they are keeping up-to-date with our puppet agent improvements.

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:


- [`puppetlabs-apache#2355`][puppetlabs-apache-pr-2355]: "fix mod_proxy_html on FreeBSD", thanks to [fraenki][fraenki]
- [`puppetlabs-apache#2353`][puppetlabs-apache-pr-2353]: "Parameterize SecRequestBodyLimitAction and SecResponseBodyLimitAction", thanks to [Vincevrp][Vincevrp]
- [`puppetlabs-apache#2350`][puppetlabs-apache-pr-2350]: "Drop deprecated a2mod type/providers", thanks to [bastelfreak][bastelfreak] and the following people who helped get it over the line ([ekohl][ekohl])
- [`puppetlabs-apache#2349`][puppetlabs-apache-pr-2349]: "disable::mpm_event: Fix module deactivation", thanks to [bastelfreak][bastelfreak]
- [`puppetlabs-apache#2346`][puppetlabs-apache-pr-2346]: "Remove executable bit from various files", thanks to [ekohl][ekohl]
- [`puppetlabs-apache#2345`][puppetlabs-apache-pr-2345]: "add LimitRequestLine parameter", thanks to [stefan-ahrefs][stefan-ahrefs]
- [`puppetlabs-apache#2339`][puppetlabs-apache-pr-2339]: "remove _module from apache::mod::unique_id name.", thanks to [mdklapwijk][mdklapwijk] and the following people who helped get it over the line ([ekohl][ekohl])
- [`puppetlabs-apache#2329`][puppetlabs-apache-pr-2329]: "Drop Apache 2.2 support", thanks to [ekohl][ekohl]
- [`puppetlabs-firewall#1096`][puppetlabs-firewall-pr-1096]: "support --nflog-size as replacement for --nflog-range", thanks to [kjetilho][kjetilho]
- [`puppetlabs-firewall#1085`][puppetlabs-firewall-pr-1085]: "package "iptables" has been replaced by "iptables-nft" on EL9", thanks to [kjetilho][kjetilho]
- [`puppetlabs-kubernetes#602`][puppetlabs-kubernetes-pr-602]: "Validate namespace parameter as DNS subdomain name", thanks to [deric][deric]
- [`puppetlabs-kubernetes#600`][puppetlabs-kubernetes-pr-600]: "Stronger type checking for $node_name", thanks to [deric][deric]
- [`puppetlabs-kubernetes#598`][puppetlabs-kubernetes-pr-598]: "Fix executing CNI addons commands (fixes #594)", thanks to [deric][deric]
- [`puppetlabs-kubernetes#597`][puppetlabs-kubernetes-pr-597]: "Support overriding containerd socket path (#596)", thanks to [deric][deric]
- [`puppetlabs-kubernetes#593`][puppetlabs-kubernetes-pr-593]: "Rewrite command line arguments parsing", thanks to [deric][deric]
- [`puppetlabs-mysql#1513`][puppetlabs-mysql-pr-1513]: "do not emit other ssl directives when ssl = false", thanks to [kjetilho][kjetilho]
- [`facterdb#260`][facterdb-pr-260]: "Release 1.20.0", thanks to [bastelfreak][bastelfreak]
- [`facterdb#259`][facterdb-pr-259]: "Add windows 2012 and 2016 facts", thanks to [davidsandilands][davidsandilands]

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-docker`][puppetlabs-docker] (`6.0.2`)
- [`puppetlabs-apache`][puppetlabs-apache] (`8.6.0`)
- [`puppetlabs-firewall`][puppetlabs-firewall] (`4.0.1`)
- [`puppetlabs-sqlserver`][puppetlabs-sqlserver] (`3.2.1`)

  [puppetlabs-docker]: https://github.com/puppetlabs/puppetlabs-docker
  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-firewall]: http://github.com/puppetlabs/puppetlabs-firewall
  [puppetlabs-sqlserver]: https://github.com/puppetlabs/puppetlabs-sqlserver
  [puppetlabs-apache-pr-2355]: https://github.com/puppetlabs/puppetlabs-apache/pull/2355
  [fraenki]: https://github.com/fraenki
  [puppetlabs-apache-pr-2353]: https://github.com/puppetlabs/puppetlabs-apache/pull/2353
  [Vincevrp]: https://github.com/Vincevrp
  [puppetlabs-apache-pr-2350]: https://github.com/puppetlabs/puppetlabs-apache/pull/2350
  [bastelfreak]: https://github.com/bastelfreak
  [ekohl]: https://github.com/ekohl
  [puppetlabs-apache-pr-2349]: https://github.com/puppetlabs/puppetlabs-apache/pull/2349
  [puppetlabs-apache-pr-2346]: https://github.com/puppetlabs/puppetlabs-apache/pull/2346
  [puppetlabs-apache-pr-2345]: https://github.com/puppetlabs/puppetlabs-apache/pull/2345
  [stefan-ahrefs]: https://github.com/stefan-ahrefs
  [puppetlabs-apache-pr-2339]: https://github.com/puppetlabs/puppetlabs-apache/pull/2339
  [mdklapwijk]: https://github.com/mdklapwijk
  [puppetlabs-apache-pr-2329]: https://github.com/puppetlabs/puppetlabs-apache/pull/2329
  [puppetlabs-firewall-pr-1096]: https://github.com/puppetlabs/puppetlabs-firewall/pull/1096
  [kjetilho]: https://github.com/kjetilho
  [puppetlabs-firewall-pr-1085]: https://github.com/puppetlabs/puppetlabs-firewall/pull/1085
  [puppetlabs-kubernetes-pr-602]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/602
  [deric]: https://github.com/deric
  [puppetlabs-kubernetes-pr-600]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/600
  [puppetlabs-kubernetes-pr-598]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/598
  [puppetlabs-kubernetes-pr-597]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/597
  [puppetlabs-kubernetes-pr-593]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/593
  [puppetlabs-mysql-pr-1513]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1513
  [puppetlabs-wsus_client-pr-188]: https://github.com/puppetlabs/puppetlabs-wsus_client/pull/188
  [facterdb-pr-260]: https://github.com/voxpupuli/facterdb/pull/260
  [facterdb-pr-259]: https://github.com/voxpupuli/facterdb/pull/259
  [davidsandilands]: https://github.com/davidsandilands
  [chelnak]: https://github.com/chelnak

---
author: "chelnak"
categories:
  - updates
date: "2022-12-16"
blog_tags: null
title: "2022-12-16: Content & Tooling Team Status Update"
---

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`device_manager#95`][device_manager-pr-95]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-accounts#429`][puppetlabs-accounts-pr-429]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-acl#269`][puppetlabs-acl-pr-269]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-apache#2356`][puppetlabs-apache-pr-2356]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-apache#2355`][puppetlabs-apache-pr-2355]: "fix mod_proxy_html on FreeBSD", thanks to [fraenki][fraenki]
- [`puppetlabs-apache#2353`][puppetlabs-apache-pr-2353]: "Parameterize SecRequestBodyLimitAction and SecResponseBodyLimitAction", thanks to [Vincevrp][Vincevrp]
- [`puppetlabs-apache#2350`][puppetlabs-apache-pr-2350]: "Drop deprecated a2mod type/providers", thanks to [bastelfreak][bastelfreak] and the following people who helped get it over the line ([ekohl][ekohl])
- [`puppetlabs-apache#2349`][puppetlabs-apache-pr-2349]: "disable::mpm_event: Fix module deactivation", thanks to [bastelfreak][bastelfreak]
- [`puppetlabs-apache#2346`][puppetlabs-apache-pr-2346]: "Remove executable bit from various files", thanks to [ekohl][ekohl]
- [`puppetlabs-apache#2345`][puppetlabs-apache-pr-2345]: "add LimitRequestLine parameter", thanks to [stefan-ahrefs][stefan-ahrefs]
- [`puppetlabs-apache#2339`][puppetlabs-apache-pr-2339]: "remove _module from apache::mod::unique_id name.", thanks to [mdklapwijk][mdklapwijk] and the following people who helped get it over the line ([ekohl][ekohl])
- [`puppetlabs-apache#2329`][puppetlabs-apache-pr-2329]: "Drop Apache 2.2 support", thanks to [ekohl][ekohl]
- [`puppetlabs-apt#1076`][puppetlabs-apt-pr-1076]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-chocolatey#306`][puppetlabs-chocolatey-pr-306]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-concat#748`][puppetlabs-concat-pr-748]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-docker#882`][puppetlabs-docker-pr-882]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-exec#205`][puppetlabs-exec-pr-205]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-facter_task#205`][puppetlabs-facter_task-pr-205]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-firewall#1101`][puppetlabs-firewall-pr-1101]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-firewall#1096`][puppetlabs-firewall-pr-1096]: "support --nflog-size as replacement for --nflog-range", thanks to [kjetilho][kjetilho]
- [`puppetlabs-firewall#1085`][puppetlabs-firewall-pr-1085]: "package "iptables" has been replaced by "iptables-nft" on EL9", thanks to [kjetilho][kjetilho]
- [`puppetlabs-haproxy#535`][puppetlabs-haproxy-pr-535]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-inifile#493`][puppetlabs-inifile-pr-493]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-java#542`][puppetlabs-java-pr-542]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-java_ks#421`][puppetlabs-java_ks-pr-421]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-kubernetes#603`][puppetlabs-kubernetes-pr-603]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-kubernetes#602`][puppetlabs-kubernetes-pr-602]: "Validate namespace parameter as DNS subdomain name", thanks to [deric][deric]
- [`puppetlabs-kubernetes#600`][puppetlabs-kubernetes-pr-600]: "Stronger type checking for $node_name", thanks to [deric][deric]
- [`puppetlabs-kubernetes#598`][puppetlabs-kubernetes-pr-598]: "Fix executing CNI addons commands (fixes #594)", thanks to [deric][deric]
- [`puppetlabs-kubernetes#597`][puppetlabs-kubernetes-pr-597]: "Support overriding containerd socket path (#596)", thanks to [deric][deric]
- [`puppetlabs-kubernetes#593`][puppetlabs-kubernetes-pr-593]: "Rewrite command line arguments parsing", thanks to [deric][deric]
- [`puppetlabs-motd#461`][puppetlabs-motd-pr-461]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-mysql#1515`][puppetlabs-mysql-pr-1515]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-mysql#1513`][puppetlabs-mysql-pr-1513]: "do not emit other ssl directives when ssl = false", thanks to [kjetilho][kjetilho]
- [`puppetlabs-ntp#661`][puppetlabs-ntp-pr-661]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-postgresql#1379`][puppetlabs-postgresql-pr-1379]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-powershell#391`][puppetlabs-powershell-pr-391]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-puppet_conf#184`][puppetlabs-puppet_conf-pr-184]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-reboot#336`][puppetlabs-reboot-pr-336]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-registry#271`][puppetlabs-registry-pr-271]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-satellite_pe_tools#193`][puppetlabs-satellite_pe_tools-pr-193]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-scheduled_task#221`][puppetlabs-scheduled_task-pr-221]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-service#224`][puppetlabs-service-pr-224]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-sqlserver#411`][puppetlabs-sqlserver-pr-411]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-stdlib#1287`][puppetlabs-stdlib-pr-1287]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-vcsrepo#580`][puppetlabs-vcsrepo-pr-580]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
- [`puppetlabs-wsus_client#188`][puppetlabs-wsus_client-pr-188]: "pdksync - (MAINT) Remove stalebot", thanks to [ia-content][ia-content]
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
  [device_manager-pr-95]: https://github.com/puppetlabs/device_manager/pull/95
  [ia-content]: https://github.com/ia-content
  [puppetlabs-accounts-pr-429]: https://github.com/puppetlabs/puppetlabs-accounts/pull/429
  [puppetlabs-acl-pr-269]: https://github.com/puppetlabs/puppetlabs-acl/pull/269
  [puppetlabs-apache-pr-2356]: https://github.com/puppetlabs/puppetlabs-apache/pull/2356
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
  [puppetlabs-apt-pr-1076]: https://github.com/puppetlabs/puppetlabs-apt/pull/1076
  [puppetlabs-chocolatey-pr-306]: https://github.com/puppetlabs/puppetlabs-chocolatey/pull/306
  [puppetlabs-concat-pr-748]: https://github.com/puppetlabs/puppetlabs-concat/pull/748
  [puppetlabs-docker-pr-882]: https://github.com/puppetlabs/puppetlabs-docker/pull/882
  [puppetlabs-exec-pr-205]: https://github.com/puppetlabs/puppetlabs-exec/pull/205
  [puppetlabs-facter_task-pr-205]: https://github.com/puppetlabs/puppetlabs-facter_task/pull/205
  [puppetlabs-firewall-pr-1101]: https://github.com/puppetlabs/puppetlabs-firewall/pull/1101
  [puppetlabs-firewall-pr-1096]: https://github.com/puppetlabs/puppetlabs-firewall/pull/1096
  [kjetilho]: https://github.com/kjetilho
  [puppetlabs-firewall-pr-1085]: https://github.com/puppetlabs/puppetlabs-firewall/pull/1085
  [puppetlabs-haproxy-pr-535]: https://github.com/puppetlabs/puppetlabs-haproxy/pull/535
  [puppetlabs-inifile-pr-493]: https://github.com/puppetlabs/puppetlabs-inifile/pull/493
  [puppetlabs-java-pr-542]: https://github.com/puppetlabs/puppetlabs-java/pull/542
  [puppetlabs-java_ks-pr-421]: https://github.com/puppetlabs/puppetlabs-java_ks/pull/421
  [puppetlabs-kubernetes-pr-603]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/603
  [puppetlabs-kubernetes-pr-602]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/602
  [deric]: https://github.com/deric
  [puppetlabs-kubernetes-pr-600]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/600
  [puppetlabs-kubernetes-pr-598]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/598
  [puppetlabs-kubernetes-pr-597]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/597
  [puppetlabs-kubernetes-pr-593]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/593
  [puppetlabs-motd-pr-461]: https://github.com/puppetlabs/puppetlabs-motd/pull/461
  [puppetlabs-mysql-pr-1515]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1515
  [puppetlabs-mysql-pr-1513]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1513
  [puppetlabs-ntp-pr-661]: https://github.com/puppetlabs/puppetlabs-ntp/pull/661
  [puppetlabs-postgresql-pr-1379]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1379
  [puppetlabs-powershell-pr-391]: https://github.com/puppetlabs/puppetlabs-powershell/pull/391
  [puppetlabs-puppet_conf-pr-184]: https://github.com/puppetlabs/puppetlabs-puppet_conf/pull/184
  [puppetlabs-reboot-pr-336]: https://github.com/puppetlabs/puppetlabs-reboot/pull/336
  [puppetlabs-registry-pr-271]: https://github.com/puppetlabs/puppetlabs-registry/pull/271
  [puppetlabs-satellite_pe_tools-pr-193]: https://github.com/puppetlabs/puppetlabs-satellite_pe_tools/pull/193
  [puppetlabs-scheduled_task-pr-221]: https://github.com/puppetlabs/puppetlabs-scheduled_task/pull/221
  [puppetlabs-service-pr-224]: https://github.com/puppetlabs/puppetlabs-service/pull/224
  [puppetlabs-sqlserver-pr-411]: https://github.com/puppetlabs/puppetlabs-sqlserver/pull/411
  [puppetlabs-stdlib-pr-1287]: https://github.com/puppetlabs/puppetlabs-stdlib/pull/1287
  [puppetlabs-vcsrepo-pr-580]: https://github.com/puppetlabs/puppetlabs-vcsrepo/pull/580
  [puppetlabs-wsus_client-pr-188]: https://github.com/puppetlabs/puppetlabs-wsus_client/pull/188
  [facterdb-pr-260]: https://github.com/voxpupuli/facterdb/pull/260
  [facterdb-pr-259]: https://github.com/voxpupuli/facterdb/pull/259
  [davidsandilands]: https://github.com/davidsandilands

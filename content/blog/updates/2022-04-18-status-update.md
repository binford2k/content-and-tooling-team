---
author: "chelnak"
categories:
  - updates
date: "2022-04-18"
blog_tags: null
title: "2022-04-18: Content & Tooling Team Status Update"
---

## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`provision#190`][provision-pr-190]: "(GH-187) Fixes abs failing provision if inventory file exists", thanks to [jpartlow][jpartlow]
- [`provision#189`][provision-pr-189]: "(maint) Allow setting of abs subdomain", thanks to [jpartlow][jpartlow]
- [`provision#188`][provision-pr-188]: "(maint) Change references to facter_task to be provision", thanks to [jpartlow][jpartlow]
- [`provision#186`][provision-pr-186]: "(maint) Add a spec case for the provision::abs task", thanks to [jpartlow][jpartlow]
- [`provision#185`][provision-pr-185]: "(bug) Fix abs checkout when 'ABS_SSH_PRIVATE_KEY' is unset", thanks to [MikaelSmith][MikaelSmith]
- [`provision#183`][provision-pr-183]: "Docker SSH forwarding port allocations", thanks to [hsnodgrass][hsnodgrass]
- [`provision#182`][provision-pr-182]: "(feat) Add ssh key support to abs ssh transport", thanks to [jpartlow][jpartlow] and the following people who helped get it over the line ([MikaelSmith][MikaelSmith], [daianamezdrea][daianamezdrea])
- [`puppetlabs-apache#2233`][puppetlabs-apache-pr-2233]: "Add support for PassengerPreloadBundler", thanks to [smortex][smortex] and the following people who helped get it over the line ([ekohl][ekohl])
- [`puppetlabs-apache#2227`][puppetlabs-apache-pr-2227]: "Restructure MPM disabling", thanks to [ekohl][ekohl]
- [`puppetlabs-apache#2226`][puppetlabs-apache-pr-2226]: "Drop Apache 2.0 compatibility code", thanks to [ekohl][ekohl]
- [`puppetlabs-apache#2216`][puppetlabs-apache-pr-2216]: "Drop Apache 2.2 support with Gentoo", thanks to [ekohl][ekohl]
- [`puppetlabs-apache#2209`][puppetlabs-apache-pr-2209]: "Show `allow_override` key in docs.", thanks to [Tamerz][Tamerz]
- [`puppetlabs-apache#2205`][puppetlabs-apache-pr-2205]: "(Modules-10646) - README link fixes", thanks to [makerling][makerling]
- [`puppetlabs-apt#1020`][puppetlabs-apt-pr-1020]: "(MODULES-11301) Don't install gnupg if not needed", thanks to [simondeziel][simondeziel]
- [`puppetlabs-apt#1017`][puppetlabs-apt-pr-1017]: "Use fact() function for all os.distro.* facts", thanks to [root-expert][root-expert] and the following people who helped get it over the line ([smortex][smortex], [kenyon][kenyon], [ekohl][ekohl])
- [`puppetlabs-apt#1016`][puppetlabs-apt-pr-1016]: "Clarify this Task runs apt-get, not apt", thanks to [kreeuwijk][kreeuwijk]
- [`puppetlabs-apt#1015`][puppetlabs-apt-pr-1015]: "(maint) Fix resource ordering when apt-transport-https is needed", thanks to [smortex][smortex]
- [`puppetlabs-apt#1014`][puppetlabs-apt-pr-1014]: "enable allow-insecure for apt::source defined types, includes new tes…", thanks to [hesco][hesco]
- [`puppetlabs-apt#1013`][puppetlabs-apt-pr-1013]: "Omit empty options in source.list template to fix MODULES-11174", thanks to [mpdude][mpdude]
- [`puppetlabs-apt#1012`][puppetlabs-apt-pr-1012]: "Replace `arm64` for `aarch64` in `::apt::source`", thanks to [mpdude][mpdude]
- [`puppetlabs-apt#1011`][puppetlabs-apt-pr-1011]: "Fixed gpg file for Ubuntu versions 21.04 and later.", thanks to [Conzar][Conzar]
- [`puppetlabs-apt#1010`][puppetlabs-apt-pr-1010]: "(MODULES-10763) Remove frequency collector", thanks to [LTangaF][LTangaF] and the following people who helped get it over the line ([daianamezdrea][daianamezdrea], [kenyon][kenyon])
- [`puppetlabs-chocolatey#276`][puppetlabs-chocolatey-pr-276]: "(MODULES-11206) Update dependencies to allow stdlib 8.x", thanks to [Sharpie][Sharpie]
- [`puppetlabs-chocolatey#273`][puppetlabs-chocolatey-pr-273]: "(MODULES-11255) Add basic tasks to manage packages", thanks to [smortex][smortex] and the following people who helped get it over the line ([michaeltlombardi][michaeltlombardi])
- [`puppetlabs-chocolatey#272`][puppetlabs-chocolatey-pr-272]: "Replace chocolatey::params with hiera data", thanks to [smortex][smortex]
- [`puppetlabs-docker#805`][puppetlabs-docker-pr-805]: "Fix idempotency when using scaling with docker-compose", thanks to [canihavethisone][canihavethisone]
- [`puppetlabs-docker#788`][puppetlabs-docker-pr-788]: "Make RedHat version check respect acknowledge_unsupported_os", thanks to [PolaricEntropy][PolaricEntropy]
- [`puppetlabs-firewall#1024`][puppetlabs-firewall-pr-1024]: "install module-init-tools on pre_setup step", thanks to [adrianiurca][adrianiurca]
- [`puppetlabs-haproxy#505`][puppetlabs-haproxy-pr-505]: "haproxy_userlist: fix empty users/groups handling.", thanks to [bzed][bzed]
- [`puppetlabs-haproxy#504`][puppetlabs-haproxy-pr-504]: "Added possibility filling description field", thanks to [michaelkoettenstorfer][michaelkoettenstorfer]
- [`puppetlabs-iis#330`][puppetlabs-iis-pr-330]: "MODULES-11188: trim physicalpath for iis_application resource", thanks to [adrianiurca][adrianiurca] and the following people who helped get it over the line ([BartoszBlizniak][BartoszBlizniak])
- [`puppetlabs-java#502`][puppetlabs-java-pr-502]: "(MODULES-11234) Support Adoptium Temurin", thanks to [dploeger][dploeger]
- [`puppetlabs-java_ks#385`][puppetlabs-java_ks-pr-385]: "Add support for certificate_content and private_key_content parameters", thanks to [hajee][hajee]
- [`puppetlabs-java_ks#383`][puppetlabs-java_ks-pr-383]: "move honeycomb key", thanks to [LivingInSyn][LivingInSyn]
- [`puppetlabs-java_ks#382`][puppetlabs-java_ks-pr-382]: "change the honeycomb writekey to a github secret", thanks to [LivingInSyn][LivingInSyn]
- [`puppetlabs-kubernetes#554`][puppetlabs-kubernetes-pr-554]: "fix: anchor regex for determining config_version", thanks to [TheMeier][TheMeier]
- [`puppetlabs-kubernetes#539`][puppetlabs-kubernetes-pr-539]: "Update dependencies", thanks to [sazzle2611][sazzle2611] and the following people who helped get it over the line ([daianamezdrea][daianamezdrea])
- [`puppetlabs-kubernetes#535`][puppetlabs-kubernetes-pr-535]: "Update Debian-family docker repo location and key id", thanks to [jorhett][jorhett] and the following people who helped get it over the line ([daianamezdrea][daianamezdrea])
- [`puppetlabs-mysql#1456`][puppetlabs-mysql-pr-1456]: "Updated db defined type strings documentation (#1)", thanks to [benjamin-robertson][benjamin-robertson]
- [`puppetlabs-mysql#1443`][puppetlabs-mysql-pr-1443]: "Test changes to exclude percona tests for scientific7 and oraclelinux7", thanks to [daianamezdrea][daianamezdrea]
- [`puppetlabs-mysql#1441`][puppetlabs-mysql-pr-1441]: "add mysql_native_password plugin to authentication_string vs password", thanks to [Heidistein][Heidistein] and the following people who helped get it over the line ([daianamezdrea][daianamezdrea])
- [`puppetlabs-ntp#628`][puppetlabs-ntp-pr-628]: "Moving plans to new acceptance folder", thanks to [sheenaajay][sheenaajay]
- [`puppetlabs-postgresql#1327`][puppetlabs-postgresql-pr-1327]: "Remove unused variable in reload.pp", thanks to [ekohl][ekohl]
- [`puppetlabs-postgresql#1323`][puppetlabs-postgresql-pr-1323]: "Fix spec tests", thanks to [ekohl][ekohl]
- [`puppetlabs-postgresql#1322`][puppetlabs-postgresql-pr-1322]: "fix spec postgresql_password with scram-sha-256", thanks to [fe80][fe80]
- [`puppetlabs-postgresql#1317`][puppetlabs-postgresql-pr-1317]: "add default version for Fedora 35", thanks to [jflorian][jflorian] and the following people who helped get it over the line ([lweller][lweller], [ekohl][ekohl])
- [`puppetlabs-postgresql#1316`][puppetlabs-postgresql-pr-1316]: "Fix python package name in RHEL/CentOS 8", thanks to [kajinamit][kajinamit] and the following people who helped get it over the line ([tobias-urdin][tobias-urdin], [ekohl][ekohl])
- [`puppetlabs-postgresql#1313`][puppetlabs-postgresql-pr-1313]: "add scram-sha-256 support", thanks to [fe80][fe80]
- [`puppetlabs-postgresql#1312`][puppetlabs-postgresql-pr-1312]: "add support for Ubuntu Hirsute and Impish", thanks to [nicholascioli][nicholascioli]
- [`puppetlabs-postgresql#1311`][puppetlabs-postgresql-pr-1311]: "Write facts as shared examples, move to Debian 11 and follow rspec-puppet path conventions", thanks to [ekohl][ekohl] and the following people who helped get it over the line ([daianamezdrea][daianamezdrea])
- [`puppetlabs-postgresql#1310`][puppetlabs-postgresql-pr-1310]: "Allow systemd to mask postgresql service file", thanks to [kim-sondrup][kim-sondrup]
- [`puppetlabs-postgresql#1309`][puppetlabs-postgresql-pr-1309]: "Make ::contrib a noop on OSes without a contrib package", thanks to [carlosduelo][carlosduelo] and the following people who helped get it over the line ([ekohl][ekohl])
- [`puppetlabs-service#203`][puppetlabs-service-pr-203]: "Create CODEOWNERS", thanks to [nmburgan][nmburgan]
- [`puppetlabs-stdlib#1231`][puppetlabs-stdlib-pr-1231]: "Fix `to_yaml` `options` parameter", thanks to [alexjfisher][alexjfisher]
- [`puppetlabs-tomcat#477`][puppetlabs-tomcat-pr-477]: "Update puppet-archive dependency", thanks to [h4l][h4l]
- [`puppetlabs-vcsrepo#527`][puppetlabs-vcsrepo-pr-527]: "MODULES-11050 - Force fetch tags", thanks to [sp-ricard-valverde][sp-ricard-valverde]
- [`facterdb#243`][facterdb-pr-243]: "Add OL6 facts for Facter 4", thanks to [as0bu][as0bu]
- [`facterdb#242`][facterdb-pr-242]: "Release 1.15.0", thanks to [bastelfreak][bastelfreak]
- [`facterdb#241`][facterdb-pr-241]: "Add opensuse 15 factsets", thanks to [bastelfreak][bastelfreak] and the following people who helped get it over the line ([smortex][smortex])
- [`facterdb#240`][facterdb-pr-240]: "Add new SLES15 facts", thanks to [tuxmea][tuxmea]
- [`facterdb#239`][facterdb-pr-239]: "Release 1.14.0", thanks to [bastelfreak][bastelfreak]
- [`facterdb#238`][facterdb-pr-238]: "Ubuntu 16: Update facter 3/4 factsets", thanks to [bastelfreak][bastelfreak]
- [`facterdb#236`][facterdb-pr-236]: "Add popos 21.10 x86_64 facts", thanks to [logicminds][logicminds] and the following people who helped get it over the line ([smortex][smortex], [bastelfreak][bastelfreak])
- [`facterdb#235`][facterdb-pr-235]: "Release 1.13.0", thanks to [bastelfreak][bastelfreak]
- [`facterdb#234`][facterdb-pr-234]: "Add CentOS Stream8/9 boxes", thanks to [bastelfreak][bastelfreak] and the following people who helped get it over the line ([traylenator][traylenator])
- [`facterdb#233`][facterdb-pr-233]: "document minimal Ruby 2.5 version in gemspec", thanks to [bastelfreak][bastelfreak]
- [`facterdb#232`][facterdb-pr-232]: "Add Ruby 3.1 to CI matrix", thanks to [bastelfreak][bastelfreak]
- [`facterdb#231`][facterdb-pr-231]: "Add CentOS 9 facter 3.14 facts", thanks to [bastelfreak][bastelfreak] and the following people who helped get it over the line ([traylenator][traylenator])
- [`facterdb#230`][facterdb-pr-230]: "Ensure all facts have osfamily/operatingsystem facts", thanks to [bastelfreak][bastelfreak]
- [`facterdb#228`][facterdb-pr-228]: "add spec tests for legacy osfamily and operatingsystem facts", thanks to [jhoblitt][jhoblitt] and the following people who helped get it over the line ([bastelfreak][bastelfreak])
- [`facterdb#227`][facterdb-pr-227]: "add a default rake target", thanks to [jhoblitt][jhoblitt] and the following people who helped get it over the line ([bastelfreak][bastelfreak])
- [`facterdb#226`][facterdb-pr-226]: "Release 1.12.2", thanks to [bastelfreak][bastelfreak]
- [`facterdb#225`][facterdb-pr-225]: "validate all factsets to legacy facts & fix renaming network related facts", thanks to [bastelfreak][bastelfreak]
- [`facterdb#224`][facterdb-pr-224]: "Validate legacy domain/fqdn/hostname fact on all factsets & Add missing fqdn/domain/hostname fact to all factsets", thanks to [bastelfreak][bastelfreak]
- [`facterdb#223`][facterdb-pr-223]: "Add test for legacy domain fact & Add/correct legacy domain fact", thanks to [bastelfreak][bastelfreak]
- [`facterdb#222`][facterdb-pr-222]: "Add test for legacy FQDN/hostname & correct FQDN/hostname facts", thanks to [bastelfreak][bastelfreak]
- [`facterdb#220`][facterdb-pr-220]: "Oraclelinux/RHEL 9: Add legacy facts", thanks to [bastelfreak][bastelfreak]
- [`facterdb#219`][facterdb-pr-219]: "Add some CentOS 9 legacy facts", thanks to [traylenator][traylenator] and the following people who helped get it over the line ([bastelfreak][bastelfreak])
- [`facterdb#218`][facterdb-pr-218]: "Adding facts for Fedora 35", thanks to [hbrown-uiowa][hbrown-uiowa]
- [`facterdb#217`][facterdb-pr-217]: "Release 1.12.1", thanks to [bastelfreak][bastelfreak]
- [`facterdb#216`][facterdb-pr-216]: "Fix hostname facts for freebsd13 and add spec test", thanks to [msalway][msalway] and the following people who helped get it over the line ([bastelfreak][bastelfreak])
- [`facterdb#214`][facterdb-pr-214]: "Release 1.12.0", thanks to [bastelfreak][bastelfreak]
- [`facterdb#213`][facterdb-pr-213]: "Cleanup stdlib/systemd facts and add tests to ensure that they are absent", thanks to [bastelfreak][bastelfreak]
- [`dependency_checker#31`][dependency_checker-pr-31]: "(GH-30) Add Forge hostname and auth token params", thanks to [sanfrancrisko][sanfrancrisko]
- [`dropsonde#19`][dropsonde-pr-19]: "Updates the telemetry endpoint to a stable URL", thanks to [MikaelSmith][MikaelSmith]
- [`dropsonde#17`][dropsonde-pr-17]: "(MAINT) Update gemspec license param to 'Apache-2.0'", thanks to [sanfrancrisko][sanfrancrisko]
- [`dropsonde#16`][dropsonde-pr-16]: "(MAINT) Release prep for 0.0.6", thanks to [sanfrancrisko][sanfrancrisko]
- [`dropsonde#15`][dropsonde-pr-15]: "(MAINT) Fix Rubocop violations", thanks to [sanfrancrisko][sanfrancrisko]
- [`dropsonde#14`][dropsonde-pr-14]: "(SERVER-3079) Allow overriding Puppet's base settings", thanks to [Magisus][Magisus]
- [`dropsonde#13`][dropsonde-pr-13]: "Load Ruby's CA certificates instead of using httpclient defaults", thanks to [Magisus][Magisus]
- [`iac#325`][iac-pr-325]: "(MAINT) Take credit and fix date for farewell post", thanks to [michaeltlombardi][michaeltlombardi]
- [`iac#324`][iac-pr-324]: "(MAINT) Draft Fond Farewell blog post", thanks to [michaeltlombardi][michaeltlombardi]
- [`iac#320`][iac-pr-320]: "(GH-319) Add `dependabot[bot]` user to excluded PRs", thanks to [sanfrancrisko][sanfrancrisko]
- [`litmus#27`][litmus-pr-27]: "Add CODEOWNERS file", thanks to [michaeltlombardi][michaeltlombardi]
- [`pdk#1159`][pdk-pr-1159]: "(Docs) Edit release note", thanks to [hestonhoffman][hestonhoffman]
- [`pdk#1158`][pdk-pr-1158]: "(PDK-1766) Prep for 2.4.0 release", thanks to [michaeltlombardi][michaeltlombardi]
- [`pdk#1154`][pdk-pr-1154]: "(PDK-1758) supplement `in_module_root` with check for `metadata.json`", thanks to [da-ar][da-ar]
- [`pdk#1152`][pdk-pr-1152]: "(PDK-1756) Bump to 2.4.0.pre", thanks to [da-ar][da-ar]
- [`pdk#1151`][pdk-pr-1151]: "(maint) bump version on homepage", thanks to [da-ar][da-ar]
- [`pdk#1150`][pdk-pr-1150]: "(maint) Docs for 2.3.0", thanks to [da-ar][da-ar]
- [`pdk#1149`][pdk-pr-1149]: "(PDK-1746) Release prep for 2.3.0 ", thanks to [da-ar][da-ar]
- [`pdk-templates#467`][pdk-templates-pr-467]: "Update README.md to show how to add more paths as validation exclusion for plan locations", thanks to [davidsandilands][davidsandilands]
- [`pdk-templates#466`][pdk-templates-pr-466]: "Update TargetrubyVersion for rubocop", thanks to [MartyEwings][MartyEwings]
- [`pdk-templates#463`][pdk-templates-pr-463]: "Use voxpupuli-puppet-lint-plugins", thanks to [bastelfreak][bastelfreak]
- [`pdk-templates#461`][pdk-templates-pr-461]: "Add a knob to allow tasks testing using ruby_task_helper", thanks to [smortex][smortex]
- [`pdk-templates#458`][pdk-templates-pr-458]: "(MODULES-11220) Disable nightly workflows on forks", thanks to [sanfrancrisko][sanfrancrisko]
- [`pdk-templates#457`][pdk-templates-pr-457]: "(GH-445,456) devcontainer updates", thanks to [da-ar][da-ar]
- [`pdk-vanagon#298`][pdk-vanagon-pr-298]: "(maint) Use choco upgrade instead of deprecated choco update", thanks to [nicklewis][nicklewis]
- [`pdk-vanagon#297`][pdk-vanagon-pr-297]: "(maint) Add support for sles15 for pdk", thanks to [underscorgan][underscorgan]
- [`pdk-vanagon#296`][pdk-vanagon-pr-296]: "(RE-13380) Set Apple notarization to false.", thanks to [jackie-kinsler][jackie-kinsler]
- [`pdk-vanagon#294`][pdk-vanagon-pr-294]: "(maint) Remove platform definitions for EOL platforms", thanks to [underscorgan][underscorgan]
- [`puppet-lint#37`][puppet-lint-pr-37]: "Extend tested-modules in CI", thanks to [bastelfreak][bastelfreak]
- [`puppet-lint#36`][puppet-lint-pr-36]: "Reenable coverage reports", thanks to [bastelfreak][bastelfreak]
- [`puppet-lint#35`][puppet-lint-pr-35]: "Don't print GitHub annotations in JSON mode", thanks to [ekohl][ekohl]
- [`puppet-lint#34`][puppet-lint-pr-34]: "Add GitHub Actions annotations", thanks to [ekohl][ekohl] and the following people who helped get it over the line ([genebean][genebean])
- [`puppet-resource_api#296`][puppet-resource_api-pr-296]: "(packaging) Sets version to 1.8.15 for release", thanks to [mhashizume][mhashizume]
- [`puppet-resource_api#294`][puppet-resource_api-pr-294]: "Add array support to autorequire variable expansion", thanks to [seanmil][seanmil] and the following people who helped get it over the line ([michaeltlombardi][michaeltlombardi])
- [`puppet-resource_api#293`][puppet-resource_api-pr-293]: "(GH-231) Add default to transport attributes", thanks to [seanmil][seanmil]
- [`puppet-resource_api#292`][puppet-resource_api-pr-292]: "Support ensure parameter with Optional data type", thanks to [seanmil][seanmil] and the following people who helped get it over the line ([michaeltlombardi][michaeltlombardi])
- [`puppet-strings#295`][puppet-strings-pr-295]: "add snyk workflow", thanks to [LivingInSyn][LivingInSyn]
- [`puppet-strings#292`][puppet-strings-pr-292]: "Release prep for v2.9.0", thanks to [sanfrancrisko][sanfrancrisko]
- [`puppet-strings#291`][puppet-strings-pr-291]: "Implement a strings:validate:reference task", thanks to [ekohl][ekohl] and the following people who helped get it over the line ([sanfrancrisko][sanfrancrisko])
- [`puppetlabs_spec_helper#347`][puppetlabs_spec_helper-pr-347]: "Configure puppet-lint to fail on warnings again", thanks to [ekohl][ekohl]
- [`rspec-puppet#22`][rspec-puppet-pr-22]: "Handle nil autorequire results", thanks to [seanmil][seanmil]
- [`rspec-puppet#21`][rspec-puppet-pr-21]: "(MAINT) Add v2.11.1 entry to docs/changelog/index.md", thanks to [sanfrancrisko][sanfrancrisko]
- [`rspec-puppet#20`][rspec-puppet-pr-20]: "(MAINT) Release prep for v2.11.1", thanks to [sanfrancrisko][sanfrancrisko]
- [`rspec-puppet#19`][rspec-puppet-pr-19]: "Ensure FacterImpl consistency between example groups", thanks to [GabrielNagy][GabrielNagy] and the following people who helped get it over the line ([bastelfreak][bastelfreak], [root-expert][root-expert])
- [`rspec-puppet#17`][rspec-puppet-pr-17]: "Release Prep for 2.11.0", thanks to [da-ar][da-ar]
- [`rspec-puppet#16`][rspec-puppet-pr-16]: "Add setting to use custom Facter implementation", thanks to [GabrielNagy][GabrielNagy] and the following people who helped get it over the line ([ekohl][ekohl], [bastelfreak][bastelfreak])

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-docker`][puppetlabs-docker] (`4.2.1`)
- [`puppetlabs-java`][puppetlabs-java] (`8.0.0`)
- [`puppetlabs-apache`][puppetlabs-apache] (`7.0.0`)
- [`puppetlabs-firewall`][puppetlabs-firewall] (`3.4.0`)
- [`puppetlabs-postgresql`][puppetlabs-postgresql] (`8.0.0`)
- [`puppetlabs-java_ks`][puppetlabs-java_ks] (`4.3.0`)
- [`puppetlabs-chocolatey`][puppetlabs-chocolatey] (`6.1.1`)
- [`puppetlabs-iis`][puppetlabs-iis] (`8.1.0`)
- [`puppetlabs-dsc_lite`][puppetlabs-dsc_lite] (`3.2.0`)

  [puppetlabs-docker]: https://github.com/puppetlabs/puppetlabs-docker
  [puppetlabs-java]: https://github.com/puppetlabs/puppetlabs-java
  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-firewall]: http://github.com/puppetlabs/puppetlabs-firewall
  [puppetlabs-postgresql]: https://github.com/puppetlabs/puppetlabs-postgresql
  [puppetlabs-java_ks]: https://github.com/puppetlabs/puppetlabs-java_ks
  [puppetlabs-chocolatey]: https://github.com/puppetlabs/puppetlabs-chocolatey
  [puppetlabs-iis]: https://github.com/puppetlabs/puppetlabs-iis
  [puppetlabs-dsc_lite]: https://github.com/puppetlabs/puppetlabs-dsc_lite
  [provision-pr-190]: https://github.com/puppetlabs/provision/pull/190
  [jpartlow]: https://github.com/jpartlow
  [provision-pr-189]: https://github.com/puppetlabs/provision/pull/189
  [provision-pr-188]: https://github.com/puppetlabs/provision/pull/188
  [provision-pr-186]: https://github.com/puppetlabs/provision/pull/186
  [provision-pr-185]: https://github.com/puppetlabs/provision/pull/185
  [MikaelSmith]: https://github.com/MikaelSmith
  [provision-pr-183]: https://github.com/puppetlabs/provision/pull/183
  [hsnodgrass]: https://github.com/hsnodgrass
  [provision-pr-182]: https://github.com/puppetlabs/provision/pull/182
  [daianamezdrea]: https://github.com/daianamezdrea
  [puppetlabs-apache-pr-2233]: https://github.com/puppetlabs/puppetlabs-apache/pull/2233
  [smortex]: https://github.com/smortex
  [ekohl]: https://github.com/ekohl
  [puppetlabs-apache-pr-2227]: https://github.com/puppetlabs/puppetlabs-apache/pull/2227
  [puppetlabs-apache-pr-2226]: https://github.com/puppetlabs/puppetlabs-apache/pull/2226
  [puppetlabs-apache-pr-2216]: https://github.com/puppetlabs/puppetlabs-apache/pull/2216
  [puppetlabs-apache-pr-2209]: https://github.com/puppetlabs/puppetlabs-apache/pull/2209
  [Tamerz]: https://github.com/Tamerz
  [puppetlabs-apache-pr-2205]: https://github.com/puppetlabs/puppetlabs-apache/pull/2205
  [makerling]: https://github.com/makerling
  [puppetlabs-apt-pr-1020]: https://github.com/puppetlabs/puppetlabs-apt/pull/1020
  [simondeziel]: https://github.com/simondeziel
  [puppetlabs-apt-pr-1017]: https://github.com/puppetlabs/puppetlabs-apt/pull/1017
  [root-expert]: https://github.com/root-expert
  [kenyon]: https://github.com/kenyon
  [puppetlabs-apt-pr-1016]: https://github.com/puppetlabs/puppetlabs-apt/pull/1016
  [kreeuwijk]: https://github.com/kreeuwijk
  [puppetlabs-apt-pr-1015]: https://github.com/puppetlabs/puppetlabs-apt/pull/1015
  [puppetlabs-apt-pr-1014]: https://github.com/puppetlabs/puppetlabs-apt/pull/1014
  [hesco]: https://github.com/hesco
  [puppetlabs-apt-pr-1013]: https://github.com/puppetlabs/puppetlabs-apt/pull/1013
  [mpdude]: https://github.com/mpdude
  [puppetlabs-apt-pr-1012]: https://github.com/puppetlabs/puppetlabs-apt/pull/1012
  [puppetlabs-apt-pr-1011]: https://github.com/puppetlabs/puppetlabs-apt/pull/1011
  [Conzar]: https://github.com/Conzar
  [puppetlabs-apt-pr-1010]: https://github.com/puppetlabs/puppetlabs-apt/pull/1010
  [LTangaF]: https://github.com/LTangaF
  [puppetlabs-chocolatey-pr-276]: https://github.com/puppetlabs/puppetlabs-chocolatey/pull/276
  [Sharpie]: https://github.com/Sharpie
  [puppetlabs-chocolatey-pr-273]: https://github.com/puppetlabs/puppetlabs-chocolatey/pull/273
  [michaeltlombardi]: https://github.com/michaeltlombardi
  [puppetlabs-chocolatey-pr-272]: https://github.com/puppetlabs/puppetlabs-chocolatey/pull/272
  [puppetlabs-docker-pr-805]: https://github.com/puppetlabs/puppetlabs-docker/pull/805
  [canihavethisone]: https://github.com/canihavethisone
  [puppetlabs-docker-pr-788]: https://github.com/puppetlabs/puppetlabs-docker/pull/788
  [PolaricEntropy]: https://github.com/PolaricEntropy
  [puppetlabs-firewall-pr-1024]: https://github.com/puppetlabs/puppetlabs-firewall/pull/1024
  [adrianiurca]: https://github.com/adrianiurca
  [puppetlabs-haproxy-pr-505]: https://github.com/puppetlabs/puppetlabs-haproxy/pull/505
  [bzed]: https://github.com/bzed
  [puppetlabs-haproxy-pr-504]: https://github.com/puppetlabs/puppetlabs-haproxy/pull/504
  [michaelkoettenstorfer]: https://github.com/michaelkoettenstorfer
  [puppetlabs-iis-pr-330]: https://github.com/puppetlabs/puppetlabs-iis/pull/330
  [BartoszBlizniak]: https://github.com/BartoszBlizniak
  [puppetlabs-java-pr-502]: https://github.com/puppetlabs/puppetlabs-java/pull/502
  [dploeger]: https://github.com/dploeger
  [puppetlabs-java_ks-pr-385]: https://github.com/puppetlabs/puppetlabs-java_ks/pull/385
  [hajee]: https://github.com/hajee
  [puppetlabs-java_ks-pr-383]: https://github.com/puppetlabs/puppetlabs-java_ks/pull/383
  [LivingInSyn]: https://github.com/LivingInSyn
  [puppetlabs-java_ks-pr-382]: https://github.com/puppetlabs/puppetlabs-java_ks/pull/382
  [puppetlabs-kubernetes-pr-554]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/554
  [TheMeier]: https://github.com/TheMeier
  [puppetlabs-kubernetes-pr-539]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/539
  [sazzle2611]: https://github.com/sazzle2611
  [puppetlabs-kubernetes-pr-535]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/535
  [jorhett]: https://github.com/jorhett
  [puppetlabs-mysql-pr-1456]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1456
  [benjamin-robertson]: https://github.com/benjamin-robertson
  [puppetlabs-mysql-pr-1443]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1443
  [puppetlabs-mysql-pr-1441]: https://github.com/puppetlabs/puppetlabs-mysql/pull/1441
  [Heidistein]: https://github.com/Heidistein
  [puppetlabs-ntp-pr-628]: https://github.com/puppetlabs/puppetlabs-ntp/pull/628
  [sheenaajay]: https://github.com/sheenaajay
  [puppetlabs-postgresql-pr-1327]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1327
  [puppetlabs-postgresql-pr-1323]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1323
  [puppetlabs-postgresql-pr-1322]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1322
  [fe80]: https://github.com/fe80
  [puppetlabs-postgresql-pr-1317]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1317
  [jflorian]: https://github.com/jflorian
  [lweller]: https://github.com/lweller
  [puppetlabs-postgresql-pr-1316]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1316
  [kajinamit]: https://github.com/kajinamit
  [tobias-urdin]: https://github.com/tobias-urdin
  [puppetlabs-postgresql-pr-1313]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1313
  [puppetlabs-postgresql-pr-1312]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1312
  [nicholascioli]: https://github.com/nicholascioli
  [puppetlabs-postgresql-pr-1311]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1311
  [puppetlabs-postgresql-pr-1310]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1310
  [kim-sondrup]: https://github.com/kim-sondrup
  [puppetlabs-postgresql-pr-1309]: https://github.com/puppetlabs/puppetlabs-postgresql/pull/1309
  [carlosduelo]: https://github.com/carlosduelo
  [puppetlabs-service-pr-203]: https://github.com/puppetlabs/puppetlabs-service/pull/203
  [nmburgan]: https://github.com/nmburgan
  [puppetlabs-stdlib-pr-1231]: https://github.com/puppetlabs/puppetlabs-stdlib/pull/1231
  [alexjfisher]: https://github.com/alexjfisher
  [puppetlabs-tomcat-pr-477]: https://github.com/puppetlabs/puppetlabs-tomcat/pull/477
  [h4l]: https://github.com/h4l
  [puppetlabs-vcsrepo-pr-527]: https://github.com/puppetlabs/puppetlabs-vcsrepo/pull/527
  [sp-ricard-valverde]: https://github.com/sp-ricard-valverde
  [facterdb-pr-243]: https://github.com/voxpupuli/facterdb/pull/243
  [as0bu]: https://github.com/as0bu
  [facterdb-pr-242]: https://github.com/voxpupuli/facterdb/pull/242
  [bastelfreak]: https://github.com/bastelfreak
  [facterdb-pr-241]: https://github.com/voxpupuli/facterdb/pull/241
  [facterdb-pr-240]: https://github.com/voxpupuli/facterdb/pull/240
  [tuxmea]: https://github.com/tuxmea
  [facterdb-pr-239]: https://github.com/voxpupuli/facterdb/pull/239
  [facterdb-pr-238]: https://github.com/voxpupuli/facterdb/pull/238
  [facterdb-pr-236]: https://github.com/voxpupuli/facterdb/pull/236
  [logicminds]: https://github.com/logicminds
  [facterdb-pr-235]: https://github.com/voxpupuli/facterdb/pull/235
  [facterdb-pr-234]: https://github.com/voxpupuli/facterdb/pull/234
  [traylenator]: https://github.com/traylenator
  [facterdb-pr-233]: https://github.com/voxpupuli/facterdb/pull/233
  [facterdb-pr-232]: https://github.com/voxpupuli/facterdb/pull/232
  [facterdb-pr-231]: https://github.com/voxpupuli/facterdb/pull/231
  [facterdb-pr-230]: https://github.com/voxpupuli/facterdb/pull/230
  [facterdb-pr-228]: https://github.com/voxpupuli/facterdb/pull/228
  [jhoblitt]: https://github.com/jhoblitt
  [facterdb-pr-227]: https://github.com/voxpupuli/facterdb/pull/227
  [facterdb-pr-226]: https://github.com/voxpupuli/facterdb/pull/226
  [facterdb-pr-225]: https://github.com/voxpupuli/facterdb/pull/225
  [facterdb-pr-224]: https://github.com/voxpupuli/facterdb/pull/224
  [facterdb-pr-223]: https://github.com/voxpupuli/facterdb/pull/223
  [facterdb-pr-222]: https://github.com/voxpupuli/facterdb/pull/222
  [facterdb-pr-220]: https://github.com/voxpupuli/facterdb/pull/220
  [facterdb-pr-219]: https://github.com/voxpupuli/facterdb/pull/219
  [facterdb-pr-218]: https://github.com/voxpupuli/facterdb/pull/218
  [hbrown-uiowa]: https://github.com/hbrown-uiowa
  [facterdb-pr-217]: https://github.com/voxpupuli/facterdb/pull/217
  [facterdb-pr-216]: https://github.com/voxpupuli/facterdb/pull/216
  [msalway]: https://github.com/msalway
  [facterdb-pr-214]: https://github.com/voxpupuli/facterdb/pull/214
  [facterdb-pr-213]: https://github.com/voxpupuli/facterdb/pull/213
  [dependency_checker-pr-31]: https://github.com/puppetlabs/dependency_checker/pull/31
  [sanfrancrisko]: https://github.com/sanfrancrisko
  [dropsonde-pr-19]: https://github.com/puppetlabs/dropsonde/pull/19
  [dropsonde-pr-17]: https://github.com/puppetlabs/dropsonde/pull/17
  [dropsonde-pr-16]: https://github.com/puppetlabs/dropsonde/pull/16
  [dropsonde-pr-15]: https://github.com/puppetlabs/dropsonde/pull/15
  [dropsonde-pr-14]: https://github.com/puppetlabs/dropsonde/pull/14
  [Magisus]: https://github.com/Magisus
  [dropsonde-pr-13]: https://github.com/puppetlabs/dropsonde/pull/13
  [iac-pr-325]: https://github.com/puppetlabs/iac/pull/325
  [iac-pr-324]: https://github.com/puppetlabs/iac/pull/324
  [iac-pr-320]: https://github.com/puppetlabs/iac/pull/320
  [litmus-pr-27]: https://github.com/puppetlabs/litmus/pull/27
  [pdk-pr-1159]: https://github.com/puppetlabs/pdk/pull/1159
  [hestonhoffman]: https://github.com/hestonhoffman
  [pdk-pr-1158]: https://github.com/puppetlabs/pdk/pull/1158
  [pdk-pr-1154]: https://github.com/puppetlabs/pdk/pull/1154
  [da-ar]: https://github.com/da-ar
  [pdk-pr-1152]: https://github.com/puppetlabs/pdk/pull/1152
  [pdk-pr-1151]: https://github.com/puppetlabs/pdk/pull/1151
  [pdk-pr-1150]: https://github.com/puppetlabs/pdk/pull/1150
  [pdk-pr-1149]: https://github.com/puppetlabs/pdk/pull/1149
  [pdk-templates-pr-467]: https://github.com/puppetlabs/pdk-templates/pull/467
  [davidsandilands]: https://github.com/davidsandilands
  [pdk-templates-pr-466]: https://github.com/puppetlabs/pdk-templates/pull/466
  [MartyEwings]: https://github.com/MartyEwings
  [pdk-templates-pr-463]: https://github.com/puppetlabs/pdk-templates/pull/463
  [pdk-templates-pr-461]: https://github.com/puppetlabs/pdk-templates/pull/461
  [pdk-templates-pr-458]: https://github.com/puppetlabs/pdk-templates/pull/458
  [pdk-templates-pr-457]: https://github.com/puppetlabs/pdk-templates/pull/457
  [pdk-vanagon-pr-298]: https://github.com/puppetlabs/pdk-vanagon/pull/298
  [nicklewis]: https://github.com/nicklewis
  [pdk-vanagon-pr-297]: https://github.com/puppetlabs/pdk-vanagon/pull/297
  [underscorgan]: https://github.com/underscorgan
  [pdk-vanagon-pr-296]: https://github.com/puppetlabs/pdk-vanagon/pull/296
  [jackie-kinsler]: https://github.com/jackie-kinsler
  [pdk-vanagon-pr-294]: https://github.com/puppetlabs/pdk-vanagon/pull/294
  [puppet-lint-pr-37]: https://github.com/puppetlabs/puppet-lint/pull/37
  [puppet-lint-pr-36]: https://github.com/puppetlabs/puppet-lint/pull/36
  [puppet-lint-pr-35]: https://github.com/puppetlabs/puppet-lint/pull/35
  [puppet-lint-pr-34]: https://github.com/puppetlabs/puppet-lint/pull/34
  [genebean]: https://github.com/genebean
  [puppet-resource_api-pr-296]: https://github.com/puppetlabs/puppet-resource_api/pull/296
  [mhashizume]: https://github.com/mhashizume
  [puppet-resource_api-pr-294]: https://github.com/puppetlabs/puppet-resource_api/pull/294
  [seanmil]: https://github.com/seanmil
  [puppet-resource_api-pr-293]: https://github.com/puppetlabs/puppet-resource_api/pull/293
  [puppet-resource_api-pr-292]: https://github.com/puppetlabs/puppet-resource_api/pull/292
  [puppet-strings-pr-295]: https://github.com/puppetlabs/puppet-strings/pull/295
  [puppet-strings-pr-292]: https://github.com/puppetlabs/puppet-strings/pull/292
  [puppet-strings-pr-291]: https://github.com/puppetlabs/puppet-strings/pull/291
  [puppetlabs_spec_helper-pr-347]: https://github.com/puppetlabs/puppetlabs_spec_helper/pull/347
  [rspec-puppet-pr-22]: https://github.com/puppetlabs/rspec-puppet/pull/22
  [rspec-puppet-pr-21]: https://github.com/puppetlabs/rspec-puppet/pull/21
  [rspec-puppet-pr-20]: https://github.com/puppetlabs/rspec-puppet/pull/20
  [rspec-puppet-pr-19]: https://github.com/puppetlabs/rspec-puppet/pull/19
  [GabrielNagy]: https://github.com/GabrielNagy
  [rspec-puppet-pr-17]: https://github.com/puppetlabs/rspec-puppet/pull/17
  [rspec-puppet-pr-16]: https://github.com/puppetlabs/rspec-puppet/pull/16

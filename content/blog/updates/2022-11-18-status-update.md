---
author: "jordanbreen28"
categories:
  - updates
date: "2022-11-17"
blog_tags: null
title: "2022-11-18: Content & Tooling Team Status Update"
---
Happy Friday everyone! Hope you are all keeping well and are beginning to wrap up warm, drink some hot chocolate and stick on some festive movies as we welcome back the darker evenings. 
<iframe src="https://giphy.com/embed/NU9BPThD9kPpDNblHO" width="480" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/christmas-snow-winter-NU9BPThD9kPpDNblHO">via GIPHY</a></p>

## Codebase Hardening
[Lukas](https://github.com/LukasAud) has been continuing his stellar work on the hardening of our module codebases. This work helps to ensure that our supported modules are protected from malicious command injection by appropriately sanisitising inputted commands.  
## Updating gem requirements for ruby 3.0/3.1
With our recent removal of puppet-module-gems from our modules, [David](https://github.com/david22swan) has been working hard behind the scenes to ensure that our modules continue to work as expected for Ruby 3.0 and 3.1. 
## Another successful community day
As always we would like to thank each of our community contributors for continuing to produce some really great Pull Requests. This week, we were able to release [puppetlabs-apache](https://github.com/puppetlabs/puppetlabs-apache) 8.4.0, and merge 5 PRs. 
## Community Contributions

We'd like to thank the following people in the Puppet Community for their contributions over this past week:

- [`puppetlabs-apache#2342`][puppetlabs-apache-pr-2342]: "Declare minimum Puppet version to be 6.24.0", thanks to [ekohl][ekohl] and the following people who helped get it over the line ([trefzer][trefzer])
- [`puppetlabs-apache#2331`][puppetlabs-apache-pr-2331]: "add maxrequestworkers parameter for mpm_worker module", thanks to [trefzer][trefzer]
- [`puppetlabs-kubernetes#589`][puppetlabs-kubernetes-pr-589]: "Fix Build docker image tooling", thanks to [BaronMsk][BaronMsk]
- [`facterdb#258`][facterdb-pr-258]: "Windows updates for facter 4.2", thanks to [davidsandilands][davidsandilands]
- [`rspec-puppet#33`][rspec-puppet-pr-33]: "Update README.md to include sensitive function", thanks to [davidsandilands][davidsandilands]

## New Module / Gem Releases

The following modules were released this week:

- [`puppetlabs-apache`][puppetlabs-apache] (`8.4.0`)

  [puppetlabs-apache]: https://github.com/puppetlabs/puppetlabs-apache
  [puppetlabs-apache-pr-2342]: https://github.com/puppetlabs/puppetlabs-apache/pull/2342
  [ekohl]: https://github.com/ekohl
  [trefzer]: https://github.com/trefzer
  [puppetlabs-apache-pr-2331]: https://github.com/puppetlabs/puppetlabs-apache/pull/2331
  [puppetlabs-kubernetes-pr-589]: https://github.com/puppetlabs/puppetlabs-kubernetes/pull/589
  [BaronMsk]: https://github.com/BaronMsk
  [facterdb-pr-258]: https://github.com/voxpupuli/facterdb/pull/258
  [davidsandilands]: https://github.com/davidsandilands
  [rspec-puppet-pr-33]: https://github.com/puppetlabs/rspec-puppet/pull/33

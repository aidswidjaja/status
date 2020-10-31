---
title: bchan is inaccessible
date: 2020-08-31 14:16:00
resolved: false
<!-- resolvedWhen: 2018-04-25 04:13:59 -->
# Possible severity levels: down, disrupted, notice
severity: down
affected:
  - bchan
  - Web server (Sydney)
  - Email server
  - CDN
  - API
section: issue
---


*Monitoring*: it appears that during the deploymnet the server was overloaded. Currently investigating how to bring it back to normal operation. https://gyazo.com/b0fe70c4e777002c9a87428ede03b58d Currently we are trying to shut down the virtual machine and deallocate it, since we can't ssh into the server.

*Investigating:* bchan is currently down due to a deployment on the production server gone wrong. I will aim to restore services soon!

And happy halloween!

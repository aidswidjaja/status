---
title: bchan is inaccessible
date: 2020-10-31 14:16:00
resolved: true
resolvedWhen: 2020-10-31 20:45:17
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

*Resolved*: thanks guys! We managed to get it back up and running by resetting the VM (haha turn your computer off and on again go brrrr) and that seems to have ironed out any problems it had before. We're still seeing slightly more latency than usual (and you may get 502 Bad Gateway errors more often) but we're hoping this evens out - we're already seeing CPU usage gradually returning to normal. For more info see this bchan thread: https://b.adrian.id.au/t/server-outage-resolved/43/2

*Monitoring*: it appears that during the deploymnet the server was overloaded. Currently investigating how to bring it back to normal operation. https://gyazo.com/b0fe70c4e777002c9a87428ede03b58d Currently we are trying to shut down the virtual machine and deallocate it, since we can't ssh into the server.

*Investigating:* bchan is currently down due to a deployment on the production server gone wrong. I will aim to restore services soon!

And happy halloween!

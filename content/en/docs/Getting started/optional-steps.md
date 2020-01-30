---
title: "Optional Steps"
linkTitle: "Optional Steps"
description: >
  Optional additional steps to supplement the default setup.
---

## Non-stock GHI

[setup.pp](https://github.com/genebean/PiWeatherRock/blob/master/setup.pp) contains some extra info that is commented out that may be useful if you are not using the stock GUI.

## Cron job for Puppet

Running the command below will tell puppet to keep things in line every 30 minutes. See https://crontab.guru/ for examples of how you could adjust the interval.

```bash
puppet resource cron 'run puppet' \
ensure=present \
command='/usr/bin/sudo /usr/bin/puppet apply /home/pi/PiWeatherRock/setup.pp' \
minute='*/30'
```

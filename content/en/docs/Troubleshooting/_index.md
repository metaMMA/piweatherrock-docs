
---
title: "Troubleshooting Information"
linkTitle: "Troubleshooting"
weight: 4
description: >
  Things to try when stuff isn't working as expected
---

Below are a couple of tips based on issues I’ve either run into myself or others have reported. Suggestions for Addison’s are welcome.

## Git permission denied

If the `git` command says `error: cannot open .git/FETCH_HEAD: Permission denied` run this to fix things and then rerun whatever you were trying to do before seeing the error:

```bash
sudo chown -R pi:pi /home/pi/PiWeatherRock
```

## Starting fresh

If you’d like to start fresh I suggest backing up your `config.py` and then running the following commands:

```bash
cd /home/pi
sudo rm -rf /home/pi/PiWeatherRock
```

After that you can start over using the installation instructions above.

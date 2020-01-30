---
title: "Getting Updates"
linkTitle: "Getting Updates"
weight: 2
description: >
  How to get the latest version of PiWeatherRock
---

If you already have this project cloned to your computer or Pi then just run these commands:

> Note that this code block includes more than just the command you type into your terminal. The command is just the bit directly after the `$`

```bash
pi@rock:~/PiWeatherRock $ git pull
# you should see some output from git here if there are any updates

pi@rock:~/PiWeatherRock $ sudo puppet apply setup.pp
# below is a sample of the type of output you may see
Notice: Compiled catalog for rock in environment production in 0.81 seconds
Notice: /Stage[main]/Main/Python::Pip[darkskylib]/Exec[pip_install_darkskylib]/returns: executed successfully
Notice: /Stage[main]/Main/Service[PiWeatherRock.service]: Triggered 'refresh' from 1 event
Notice: Applied catalog in 115.65 seconds
```

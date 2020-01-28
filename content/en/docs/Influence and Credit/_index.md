
---
title: "Influence and Credit"
linkTitle: "Influence & Credit"
weight: 6
description: >
  Ways to get help
---

There is a lot of my own work in this project but I could have never done it without being able to build on the work of other. Below is some information about what other works have helped PiWeatherRock become what it is today.

## Weather.py - A PyGame-based weather data/forecast display

- The bulk of this project originated with the code written by Jim Kemp and published at http://www.instructables.com/id/Raspberry-Pi-Internet-Weather-Station/.
- Jim Kemp's version pulled from weather.com via pywapi but that doesn't seem seem to work any longer. This project switched pulling from Weather Underground but their API has since been made not free. As a result, this project now pulls from Dark Sky.
- Some ideas were also taken from https://github.com/sarnold/pitft-weather-display.

## Icons

Almost all the icons have been replaced with ones from [github.com/manifestinteractive/weather-underground-icons](https://github.com/manifestinteractive/weather-underground-icons/tree/47aca0a69c1246d80ee1b915c4f9906adbaa1e1b).

Some additional icons come from [erikflowers.github.io/weather-icons](https://erikflowers.github.io/weather-icons/). These have been converted to png files via the [generate-dark-sky-pngs.sh](https://github.com/genebean/PiWeatherRock/blob/master/icons/alt_icons/generate-dark-sky-pngs.sh) script. To use the script you will need to first run `pip3 install cairosvg`.

## GPIOmock.py

Pulled GPIOmock.py from [github.com/grantwinney/52-Weeks-of-Pi](https://github.com/grantwinney/52-Weeks-of-Pi/blob/b4df240bfb224b1c027c9adf71cac8159286aade/GPIOmock.py) to enable testing in an x86 virtual machine.

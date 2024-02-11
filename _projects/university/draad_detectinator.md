---
layout: post
title: Detecting cables through a wall
description: Building a measurement device to measure the depth of electricity cables in the walls.
img: /assets/projects/draad_detectinator/thumbnail.jpg
date: 2022-11-04
importance: 20221104
category: university
---

*By Timo Hoogenbosch, Luc Koster, Simon ten Dam, and Remi van den Berg.*

You can read the full report (in Dutch) [here](/assets/projects/draad_detectinator/verslag.pdf).

The device contains a microcontroller for doing the measurement. The result of the measurement is sent to a webserver, so it can be shown during a presentation. The code for the internal microcontroller, the website back-end, and the website front-end can be found here:
{% include repository/repo.liquid repository="Hoog3059/DraadDetectinator" %}
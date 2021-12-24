---
layout: post
title:  "Progress update"
date:   2019-04-01 12:00:00 +0200
categories: news
---

Progress update
===

We have quite a few things that have happened since the last update. Unfortunatelly, the code is not stable enough for a release on Apil 1st, as originally planned, but shouldn't be long now.

fh/mymaster merge
---
One of the most important changes is that Flyinghead's work is now merged in reicast master. Flyinghead has been working
on his branch for quite some time, fixing things and adding features. 

Overall, this change brings

- Save States
- Much improved NAOMI support, with support for mame rom format
- Arm64 support for both of the main cpu and the sound cpu
- Major improvements in the x64 cpu dynarec
- Improved DSP support, wich is now portable, and optimizations for arm64
- OpenGL 4.1 renderer, with sorting for transparent polygons
- Lightgun support
- A lot of bug fixes in the peripheral hardware
- Modem emulation
- Texture replacement feature for the renderers
- An imgui that is shared between android and desktop
- Many other things


Imgui ui
---
We're moving to an imgui based UI. It's not as pretty as the old UI yet, but we can use share it between desktop and mobile.


Desktop support
---
Windows + Linux
OGL4.1 renderer

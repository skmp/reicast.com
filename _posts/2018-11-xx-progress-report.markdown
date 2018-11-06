---
layout: post
title:  "Progress report September and October"
date:   2018-11-xx xx:xx:xx +0100
categories: news
---

September and October were busy as usual. We fixed some stuff and also added some new features.
We unfortunatly missed our goal to release 18.10 in October so we now try to get 18.11 out, so stay tuned for the next feature report.

Versioning [#1396](https://github.com/reicast/reicast-emulator/pull/1396)
---
We unified the display of the version for Android, Linux and Windows targets.
Using Android the version is displayed in the about dialog (see screenshot) using Windows and Linux there is the new command line switch ``-version``.
![Android version](/_images/2018-11_1396_version.png "Android version")
[add screenshot]

Emulation
---
Thanks to [@flyinghead](https://github.com/flyinghead) we fixed many emulation related bugs and implemented new features.

- Detect TA overruns and cancel the rendering. Increase TA data size [#1408](https://github.com/reicast/reicast-emulator/pull/1408) fixes crashes in D2 and Triggerheart Exelica.
- Do not crash on unaligned VRAM read access which fixes House of the Dead 2. [#1426](https://github.com/reicast/reicast-emulator/pull/1426)
- Do not crash on TA data without calling ListInit first which fixes Looney Tunes Space Race, Test Drive Le Mans and others. [#1427](https://github.com/reicast/reicast-emulator/pull/1427)
- Fix FTRC (ipr, canonical, x86) by using correct positive cutoff value which fixes wrong car color in Tokyo Xtreme Racer car selection screen. [#1428](https://github.com/reicast/reicast-emulator/pull/1428)
- Schedule the interrupt signaling the end of an Aica DMA transfer which fixes Street Fighter Alpha 3 and Bomberman Online. [#1412](https://github.com/reicast/reicast-emulator/pull/1412)

Android
---
[@AbandonedCart](https://github.com/AbandonedCart) implemented theming into the Android GUI. ([#1407](https://github.com/reicast/reicast-emulator/pull/1407), [#1413](https://github.com/reicast/reicast-emulator/pull/1413), [#1415](https://github.com/reicast/reicast-emulator/pull/1415), [#1416](https://github.com/reicast/reicast-emulator/pull/1416), [#1418](https://github.com/reicast/reicast-emulator/pull/1418), [#1419](https://github.com/reicast/reicast-emulator/pull/1419) and more)
![Android theming](/_images/2018-11_1407_theming.png "Android theming")
He also updated the Dropbox API from 1.6 to 3.0 which should fix the Dropbox Cloud-VMU support. ([#1425](https://github.com/reicast/reicast-emulator/pull/1425))

Linux
---
If there was an error initializing an evdev device under Linux, reicast would crash on startup. ([#1395](https://github.com/reicast/reicast-emulator/pull/1395))

That's it for September and October,

team reicast

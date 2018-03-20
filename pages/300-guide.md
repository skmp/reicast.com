---
layout: page
title: User guide
permalink: /getting-started/
---

[Getting started videos](https://www.youtube.com/results?search_query=Setting+up+reicast+android)
---

There are a lot of video tutorials on youtube, by many nice people. [Watch one of them!](https://www.youtube.com/results?search_query=Setting+up+reicast+android). *Keep in mind these are not officially endorsed by the reicast team*

BIOS Setup
---

You will need the Dreamcast BIOS files (dc_boot.bin and dc_flash.bin) to run reicast. You need to dump these files from your Dreamcast. We will not teach how to dump or otherwise obtain those files, so please do not ask. Google is your friend.

After you get the BIOS files, create a folder called “dc” at the top level of your SD card partition (the name can vary per device, note that this is not the external SD card partition, it’s part of the internal flash). Inside there create a folder called “data” and put the BIOS files inside. Make sure that the names of the folders and the BIOS files are correct! reicast requires proper Dreamcast BIOS files! Just creating some random files and renaming them will (obviously) not work!

On newer versions of reicast you can pinpoint to the folder that contains the data folder. Just make sure that you don’t select the “data” folder, you must choose the folder containing it, Also make sure that the file names of the BIOS and flash files are correct.
Some devices do not support writing to external storage. It would be a good idea to place the aforementioned folders on the internal memory of your device in order to avoid possible issues.


How to set the time
---

If you want the BIOS to stop asking you to set the time on each launch you can follow these steps.

- Launch the bios and enter the date/time - make sure it is 5 minutes before your current local time
- Quit the bios (close the emulator)
- Boot the bios again - you should now see the time to be your correct local time!


How to Save
---

You need to format the memory card before being able to save. Here’s how to do it:

- Launch the bios and go to the memory card (vmu) screen
- Select the memory cards you want and do a complete erase (format) on them
- Quit the bios (close the emulator). You should be able to save from now on


Games
---

reicast does not come with games. You need to dump those yourself. reicast supports the following formats of Dreamcast disc dumps: gdi, cdi, chd (compressed images, only chd images up to version 4 are supported, chd version 5 images are NOT supported). Again, do not ask how to dump or obtain games. Google is your friend (again).

Usage
---

Configuration menu
===

You can access it by touching the reicast logo on the top left side of the screen or pressing left on the D-pad/analog stick of your gamepad.

- The “Browser” option sends you back to the reicast game browser.
- The “Settings” screen allows you to enable the following settings:


**Unstable optimizations** (off by default): This enables some optimizations that are not properly implemented yet. The unfinished parts are hacked together until their implementation is finished. This makes the optimizations unstable.
Turning this option ON makes things faster, but also makes the emulator more unstable.


**Limit FPS** (on by default): This enables the internal frame limiter.
Turning this ON makes reicast stop from running too fast.


**Use mipmaps** (on by default): This enables emulation of MIPMAPS. This is meant to be always ON and not have a configuration option. Unfortunately some driver bugs for PowerVR SGX produce GFX artifacts when this is used. Thus, the need for this option.
Disabling the option if your device has a PowerVR SGX and textures appear messed up will (most likely) fix the errors.


**Widescreen mode** (off by default): This is a hack that makes the system output graphics on the whole screen. Some games actually work fine with it, while others show artifacts.
This should be normally OFF. If a game actually works fine with it set ON, then you might want to use it.


**Frameskip value** (0 by default): This makes reicast skip processing and rendering some frames, in hopes of running a bit faster.
Set this option to 0 unless reicast runs really slow. In that case, you might want to increase it a bit.

Paths
===

The “Paths” screen allows you to tell reicast where the folder with your BIOS files and where the folder with your game files are placed.

Note: When selecting where you BIOS files are, do not select the “data” folder. Select the folder that has the “data” folder inside it!
For example, if the path is “/mnt/sdcard/dc/data/” then you need to choose the “dc” folder.

Input
===

The “Input” screen allows you to select and assign the controllers you want to use with reicast.

Note that while some controllers are supported by reicast, some others are not. Be sure to let us know if your controller is supported!
If your device has a microphone you can enable one microphone device to be “plugged in” to the second port of the first controller!

About
===
The “About” screen just shows some information regarding reicast.

In-game menu
---

This can be accessed by pressing back, menu, select on your device

Top level of icons

- VMU LCD screen: This shows you the output of the LCD on the first VMU device on controller 1. Tap it to relocate it from the menu to stay on the top right of the screen! Tap that to put it back.
- **Up arrow**: closes menu
- **VMU swap**: swaps VMU 1 and 2
- **Toggle right analog stick function**: Either Y axis controls L/R triggers or the four directions control the face buttons.
- **Open runtime settings**
- **Open debug settings**
- **Close emulator**

**Runtime Settings**

- **Up arrow**: go back to top level of the menu
- **Toggle widescreen**
- **Reduce frameskip**
- **Increase frameskip**
- **Toggle Limit FPS setting**
- **Mute sound**
- **TURBO MODE**
- **Close menu**

**Debug Settings**

- Kill texture cache
- Profiler start
- Profiler stop
- Print stats
- Close menu

On-Screen Buttons
---

If you are updating from r5 to r6 there are new images for the on-screen buttons, but you will need to delete /dc/data/buttons.png to see them!
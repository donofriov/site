---
title: "Setup Raspberry Pi Operating System Boot Drive(s)"
date: 2021-02-09T13:05:46+01:00
draft: false
---


Download [Etcher](https://www.balena.io/etcher/)

![etcher home](/img/etcher.png)

Download [Raspberry Pi OS Lite](https://www.raspberrypi.org/software/operating-systems/#raspberry-pi-os-32-bit)

- Since this will be a kubernetes node, I don't need the Raspberry Pi dektop installed
- Unzip the downloaded file

![raspberry pi os lite download](/img/raspberry-pi-os-lite-download.png)

Insert SD card into SD card reader (SanDisk Extreme 32 GB A1 U3)

Etcher Steps

- Click Flash from file
- Select the downloaded `.img` file
- Click target (the SD card)
- Click Flash! (enter password if needed and accept permission requets)

Setup ssh

- Eject and re-instert SD card
- Run `touch /Volumes/boot/ssh`
- Eject SD card

Repeat SD card steps for as many Raspberry Pi nodes as needed. I'm using three.

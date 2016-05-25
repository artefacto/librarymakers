---
layout: post
title: Installing NOOBS on a Raspberry Pi
categories: [recipes]
tags: [raspberrypi, linux]
---

## Intro
Raspberry Pis are effectively fully functional mini-computers but they come without an operating system so there’s not much you can do without first installing one.

Luckily there’s been various tools created to make this easier. NOOBS stands for New Out Of the Box Software and it’s an install manager for the Raspberry Pi.

To install NOOBS on the Raspberry Pi, you have to install it on a bootable SD card. It’s recommended to have an SD card with at least 4gb space on it but different uses require different sizes so go for something at least 8gb if you can.

## What you need

- An SD card (at least 4gb) formatted as FAT32
- NOOBS files downloaded


## How

### Format an SD card (at least 4GB) as FAT.

The way you format an SD card is different on Macs, Windows or Linux computers. For Macs, you can open the Disk Utility app (Applications/Utilities), select the SD card from the list of available drives and select the erase option. Here, you can choose how to reformat the disk. Set it to MS-DOS (FAT) (see below).

![Formatting an SD Card]({{ base.url }}/public/images/format-sd-card-mac.png)


For Windows, you need to download a formatting tool like using the SD Association's Formatting Tool, available from sdcard.org. Linux users, you know what to do - http://qdosmsq.dunbar-it.co.uk/blog/2013/06/noobs-for-raspberry-pi/ ;-)

### Save the files to the SD card

- Download the NOOBS files from [(https://www.raspberrypi.org/downloads)]
- Unzip the files
- Move the files onto the SD card. They need to be in the root directory, so make sure they’re not in a subfolder.

### Boot the Pi
- You can now insert the SD card in the raspberry pi and connect it to a monitor to run the installer.

## More info

http://www.raspberrypi.org/help/noobs-setup/

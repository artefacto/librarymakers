---
layout: post
title: Raspberry Pi Digital Signage with Screenly
categories: [recipes]
tags: [raspberrypi, signage, digital signage]
---

## Intro
You can use a Raspberry Pi attached to a monitor or TV as a affordable digital signage solution to display websites, images or videos. In this example, we use Screenly OS to create a simple digital signage solution.


## What you need
 - Raspberry Pi with internet connection
 - SD card (at least 8gb)
 - HDMI cable
 - Monitor with HDMI input


## How
Download the Screenly image from :

[https://github.com/wireload/screenly-ose/releases](https://github.com/wireload/screenly-ose/releases)

To copy this on to your SD card, you can follow the instructions here.

[https://www.raspberrypi.org/documentation/installation/installing-images/](https://www.raspberrypi.org/documentation/installation/installing-images/)

When you boot up the Raspberry Pi with your Screenly SD card, you should see a welcome screen that displays the local IP address that you can access the Screenly configuration interface. This is general something like

    192.168.0.x:8080

You can then navigate to this address from any computer on the local network to start configuring your digital display.

When you open the Screenly manager, you will be able to add and remove 'assets' to display on your digital display. These can be either images, videos or webpages and will work best if sized for a 1920x1080 display.

They can be uploaded from your computer or added by URL.

![Screenly OSE manager]({{ base.url }}/public/images/screenly/Screenly-add-asset.png)

You can also edit the assets to change how long they display for and set an expiry date for a particular display.

![Screenly settings]({{ base.url }}/public/images/screenly/Screenly-manager1.png)

## More info
- [https://www.screenly.io/ose/](https://www.screenly.io/ose/)

## Where to next

- [https://www.raspberrypi.org/forums/viewtopic.php?f=41&t=12396](Screenly OSE -- Digital Signage for the Raspberry Pi) - Screenly OSE thread on the Raspberry Pi forum.

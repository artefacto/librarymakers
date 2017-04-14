---
layout: post
title: Creating a Full screen display with Raspberry Pi
categories: [recipes]
tags: [raspberrypi, display, browser]
---

## Intro

The Raspberry Pi can be a great way to have a low-cost, low-powered display to create a display that can then be updated remotely.

If you are using your Raspberry Pi with a monitor to display a website, dashboard or calendar or something you don’t want it to appear n a browser with the full desktop visible. It also helps to have it autoboot.

In this tutorial, we'll set up a calendar display that automatically launches in fullscreen mode. This fullscreen mode is often called *kiosk mode*. 

## What you need

- Raspberry Pi 2 or 3 with internet connection
- HDMI monitor

## How

Raspberry Pi comes with Midori browser by default so first, let’s install a browser that works better for full-screen (and is compatible with Google Calendar).

First, make sure you’re all up to date

    sudo apt-get update && sudo apt-get upgrade -y

Then install either Chromium or Iceweasel (forks of Google Chrome and Firefox respectively).

For Chromium:
    sudo apt-get install chromium x11-xserver-utils unclutter

For Iceweasel
    sudo apt-get install iceweasel

Open a site in the browser in ‘kiosk’ mode.

    chromium --kiosk http://my-site-address.com

To escape kiosk mode, press  ALT/F4 keys together.

Once we've tested our link and browser in kiosk mode we can start to set it up to autoboot.

First, we need to disable the screensaver and power saver modes to stop the monitor switching off all the time.

To do this we need to edit the autostart settings. This command will open the file in the nano text editor.

    sudo nano /etc/xdg/lxsession/LXDE/autostart

(on some versions of raspbian, this will be sudo nano /etc/xdg/lxsession/LXDE-pi/autostart)

Comment out the line about the screensaver by adding a hash symbol before it.

    @xscreensaver -no-splash

So, it should now be

    #@xscreensaver -no-splash

Then add these lines underneath this one:

    @xset s off
    @xset -dpms
    @xset s noblank

We now want to make sure our chosen browser autostarts when we start our Raspberry Pi

add @iceweasel (or @chromium) to the list

If you want your browser to autostart in kiosk mode, you can the full instruction here:
e.g.
@chromium --noerrdialogs --kiosk http://my-site-address.com

presss Ctrl x to exit the file and Y to save your changes

Now when you reboot, your Raspberry Pi should open the website in kiosk mode automatically.

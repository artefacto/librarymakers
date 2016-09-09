---
layout: post
title: Accessing your Raspberry Pi remotely using tightvncserver
categories: [recipes]
tags: [raspberrypi, remote, headless]
---

## Intro
If you don't have access to a monitor and keyboard or just because it can be more convenient, you may want to access your Raspberry Pi from your laptop or desktop computer.

There are a few different ways to do this but in this tutorial we're going to log in and access our Raspberry Pi remotely using Virtual Network Computing (VNC). VNC is a way of sharing desktops so you can remotely control another computer.

TightVNC is a cross-platform ,open-source remote desktop software application.


## What you need

- Raspberry Pi 2 or 3 with internet connection

## How

First, make sure everything is up to date on your Raspberry Pi by running:

    sudo apt-get update
    sudo apt-get upgrade

Now, we need to install the TightVNC server package from the command line by running:

    sudo apt-get install tightvncserver

Next, start the VNC server. You can also specify the dimensions of the graphical view of the remote desktop:

    tightvncserver :1 -geometry 1024x640 -depth 24 -dpi 64


Now, back to your main computer. Download a VNC viewer to your computer. There's a list of available options listed at:

[ https://www.realvnc.com/download/viewer/]( https://www.realvnc.com/download/viewer/)

It should direct you to the most popular choice for your operating system.

For Mac, it's VNC Viewer.

![VNC Viewer 1]({{ base.url }}/public/images/raspberrypi/vnc_viewer_download.png)


When you open up *VNC Viewer*, you will be prompted to log in to your Raspberry Pi using the IP address and the Display number (which is likely set to 1 unless you specified otherwise)

![VNC Viewer 2]({{ base.url }}/public/images/raspberrypi/vnc_viewer_login_1.png)


And then, finally, set the 8 character password you set for the VNC server .

And huzzah.

You will then have access to your Raspberry Pi desktop. It won't be fullscreen but it's still a lot easier to navigate than SSH or other non-graphical ways.


![VNC Viewer 3]({{ base.url }}/public/images/raspberrypi/VNC_Viewer_PI_Deskopt.png)

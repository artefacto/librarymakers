---
layout: post
title: Getting started with Sonic Pi
categories: [recipes]
tags: [raspberrypi, music, coding, sonicpi]
---

## Installing SonicPi

SonicPi comes installed on the latest versions of Raspbian (the Debian flavour created for the Raspberry Pi) but you can also install it directly on earlier versions by typing the following command at the command line.

    $ sudo apt-get install sonic-pi

Once installed you can access Sonic Pi via the desktop:

    $ type startx

There are also versions available for Windows, Mac and Linux that you can download from [http://sonic-pi.net/](http://sonic-pi.net/)

![Sonic Pi welcome]({{ base.url }}/public/images/sonic-pi/welcome-screen.png)

## The official tutorial

The first thing you’ll notice when you first launch Sonic Pi is that it directs you to a tutorial. You can access the different parts of the tutorial from the bottom pane, underneath the main code editor panel.

![Sonic Pi tutorial]({{ base.url }}/public/images/sonic-pi/Tutorial-pane-annotated.png)

This tutorial will introduce you to the Sonic Pi and the different parts of the Sonic Pi interface. It will also walk you through your first program and help you learn a bit about coding in Sonic Pi.


## The interface

The main parts of the Sonic Pi interface are the Code Editor, the main menu, the Help panel and the Log Viewer.

![Sonic Pi interface]({{ base.url }}/public/images/sonic-pi/sonic-pi-interface.png)

The Run and Stop buttons in the main menu are how you start and stop your script. In the main menu, you can also save and open files, open and close the help panel and change your preferences configuration.

![Sonic Pi menu]({{ base.url }}/public/images/sonic-pi/main-menu.png)

You can see the output of your running program in the Log Viewer.

![Sonic Pi Log Viewer]({{ base.url }}/public/images/sonic-pi/log-panel.png)

As well as showing you what the code is running, the log window will also tell you if there are any errors.

![Sonic Pi error]({{ base.url }}/public/images/sonic-pi/log-error-display.png)

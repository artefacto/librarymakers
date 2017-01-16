---
layout: post
title: Raspberry Pi Digital Signage with Pi Presents
categories: [recipes]
tags: [raspberrypi, signage, digital signage]
---

## Intro
You can use a Raspberry Pi attached to a monitor or TV as a affordable digital signage solution to display websites, images or videos. In this example, we use Pi Presents to create a multimedia digital signage solution.

This can be used to create touchscreen systems, button controlled kiosk displays, repeating multimedia shows, audio-visual interpretation of exhibits and lots more.

## What you need
 - Raspberry Pi with internet connection
 - SD card (at least 8gb) with NOOBS or Rasbian Jessie installed
 - HDMI cable
 - Monitor with HDMI input

## How

First, make sure your Raspberry Pi is up-to-date and install the required software. Pi Presents requires the Python Imaging Library (PIL), MPlayer, Uzbl webkit browser and the X server utilties package.

We will also install _unclutter_ to stop the  mouse cursor from getting in the way on our displays.

    sudo apt-get update
    sudo apt-get install python-imaging
    sudo apt-get install python-imaging-tk
    sudo apt-get install x11-xserver-utils
    sudo apt-get install unclutter
    sudo apt-get install mplayer
    sudo apt-get install uzbl

We also need to install [pexpect](https://github.com/KenT2/pipresents-next), which is a 'Python module for controlling interactive programs in a pseudo-terminal'.


     wget http://pexpect.sourceforge.net/pexpect-2.3.tar.gz
     tar xzf pexpect-2.3.tar.gz
     cd pexpect-2.3
     sudo python ./setup.py install

Next, we can download and extract PiPresents-Next.

This needs to be down from the Raspberry Pi desktop interface (either Pixel or startx). Open the terminal application and then run:

     wget https://github.com/KenT2/pipresents-next/tarball/master -O - | tar xz

You should now have a new directory available with the version number. You can rename it to _pipresents_ to make it easier to access. e.g.

    mv KenT2-pipresents-next-aa66e61 pipresents


  Then navigate into your pipresents folder and run the python file:

      cd pipresents
      python pipresents.py

Ok, so now it’s installed, we need to create some profiles to use.

There’s an example profile you can download that includes a multimedia slideshow with music, text and graphics. It’s a good basis to use for your own profile, particularly when you’re just getting started.

There are also many profile exameples and exenstive documentaiton [available in the manual](https://github.com/KenT2/pipresents-next/blob/master/manual.pdf) (PDF)


## More info

These instructions have been based on (and tested from)

[https://github.com/KenT2/pipresents-next](https://github.com/KenT2/pipresents-next)

Full Pi Presents Manual - [https://github.com/KenT2/pipresents-next/blob/master/manual.pdf](https://github.com/KenT2/pipresents-next/blob/master/manual.pdf)

## Where to next

- [Pi Presents website](https://pipresents.wordpress.com/)

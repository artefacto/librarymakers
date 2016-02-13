---
layout: post
title: Using the command line on Raspberry Pi
categories: [recipes, beginners]
tags: [CLI, raspberryPi, command-line]
---

## Intro

If you haven’t used a command line interface (CLI) before, you might be a bit lost when you first start up your Raspberry Pi and you see a login screen like this:

![Raspberry Pi boot screen]({{ base.url }}/public/images/RaspberryPi_boot.png)

Most the time, when using computers, we are accessing them using a Graphical User Interface (GUI). So, when you start your laptop, you see a Windows or Mac login screen or your Desktop layout.

This command line is a text-based interface for sending commands instead of a graphical one.  Before computers could support graphics, users interacted with them via the terminal or command line and this is still available and commonly used in non-graphical environments such as servers.


## How

The default username to log in to a raspberry pi is `pi` and the password is `raspberry`. Once you’ve logged in, you will see that the command line prompt now starts with `pi@raspberrypi`.

You can now use the raspberry pi using terminal commands or boot the Pi into its GUI Desktop by typing `startx`.

### Other basic commands

To change directory, used the cd command

`cd /home/pi`

To change directory to the parent directory

`cd ..`

To list the directories and files for the current directory

`ls`

To make a new directory

`mkdir myNewDirectory`

to change into the new directory would then be:

`cd myNewDirectory`

To shut down the Rasberry Pi

`sudo poweroff`

To reboot

`sudo reboot`

 To start the GUI desktop

`startx`

Apt-get is the command-line tool for managing packages for Debian Linux

To download a package from the package directory

`apt-get packagename`

To download and install

`apt-get install packagename`

To uninstall a package

`apt-get remove packagename`

*Nb you can use the up and down arrow keys to navigate through previous commands*

## More info

[Raspberry Pi documentation - terminal](https://www.raspberrypi.org/documentation/usage/terminal/
)

[CLI Spells for the Raspberry Pi](http://elinux.org/CLI_Spells_for_the_Raspberry_Pi
)

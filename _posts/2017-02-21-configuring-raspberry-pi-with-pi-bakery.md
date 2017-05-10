---
layout: post
title: Configuring a Raspberry Pi with PiBakery
categories: [recipes]
thumb: RaspberryPi_thumbnail_2.png
img: RaspberryPi_Scale.jpg
tags: [raspberrypi, configuration, tools]
---

## Intro
_PiBakery_ is a tool that provides a visual, drag and drop interface for configuring the Raspbian operating system for your Raspberry Pi.

It's developed by David Ferguson and is available for Mac or Windows (or source).

<!--more-->
With PiBakery, you can easily configure your Raspberry Pi operating system just the way you like it, including startup scripts and your default account. This means it's also useful for creating multiple copies of the same Raspberry Pi operating system - great for teaching and for running Raspberry Pi workshops.

## What you need

 - Mac or Windows computer (with a decent amount of hard drive space available)
 - SD card (at least 8gb) formatted.

## How

### Setting up your PiBakery
- First, download the PiBakery software from [http://www.pibakery.org/download.html](http://www.pibakery.org/download.html).
Nb. It's quite a big file as it includes versions of the Rasbian operating system that you wish to use.
- Click on the installer. This will walk you through the installation process, including where you install PiBakery.
- Choose what versions of Raspbian to install, you can install either the full Raspbian with Pixel image or Raspbian Lite (Raspbian Jessie at the time of writing).

![PiBakery install]({{ base.url }}/assets/img/blog/pibakery/pibakery-installation.png)

- You can go through the different tabs to configure Rasbian including

  - **Startup** - programs or scripts to run when the Raspberry Pi first boots up. This can be on the first boot only or every time the Raspberry Pi starts
  - **Programs** - Any additional software packages to install, Enable VNC Server or install Apache/PHP/mySQL.
  - **Network** - Set your Pi to automatically connect to a wifi network.
  - **Settings** - Change the default user password, run cron jobs or set your pi to boot to console by default.
  - **PiZero OTG** - OTG modes on the Raspberry Pi Zero.
  - **Other** - These include changing directory permissions, running python scripts as a particular user, rebooting or removing files or folders.

  ![PiBakery other options]({{ base.url }}/assets/img/blog/pibakery/pibakery-other-options.png)


- You can drag and drop these configuration blocks into a configuration file that can be exported or saved for future use.

  So, for example, if you want to clean your Rasbian installation after every workshop you run, you might end up with a script that looks like this:

  ![PiBakery script example]({{ base.url }}/assets/img/blog/pibakery/pibakery-script-example-2.png)

- You can then insert your SD card and save the customised operating system to the SD card to be used with your SD card. Click on the Write button in the top right corner. A popup window will prompt you to choose the SD card to write to.

- **Be extra careful when you're writing to the SD card that you have the correct drive selected. You don't want to overwrite another drive by mistake!**.

 If all goes well, you should now see the success message which means your SD card is all set to use with your Raspberry Pi.

   ![PiBakery success]({{ base.url }}/assets/img/blog/pibakery/pibakery-write-successful.png)

The great thing is, you can continue to update and modify your configuration settings via your Windows or Mac computer. So if things aren't quite right, you can come back and easily make any changes required.

### Changing your configuration options on an existing Rasbian installation
- Open PiBakery and insert your SD card. This will recognise your previous PiBakery configuration and an alert will appear to ask if you want to update the SD card. Select Yes to continue.  
- PiBakery will load your previous configuration options. Now you can make any changes to the configuration settings that you want. You can also add new blocks.  
- Click on 'Update' to save the new configuration.


## More info
- [PiBakery documentation](http://www.pibakery.org/docs/index.html)


## Where to next

- [Pi Bakery website](http://www.pibakery.org/)

---
layout: post
title: Controlling movement of your favourite Scratch character with PicoBoard Slider
categories: [recipes]
tags: [picoboard, scratch]
---

## Intro
After you [set-up your PicoBoard](/ingredients-picoboard), you can start playing with its different features.

In this tutorial you'll learn how to use the PicoBoard slider to control movement of a character or Sprite in Scratch. We show you how to control the character's vertical or horizontal position with the slider and how to watch the changes of the slider sensor's value in real-time.

## What you need
- PicoBoard (including mini USB cable)
- Scratch software

## How
* First of all, connect the PicoBoard with your computer with the USB cable provided in your purchased kit. We assume that your PicoBoard is set-up (all the drivers and plug-ins downloaded). If not, click here to follow the instructions how to set up your PicoBoard.
* Once everything is set up, we'll start a new project. First, we want to write a script which will allow us to control the character's movement with the slider. In this case, we want to control its vertical position.
* In Scripts, click on 'Events' button to select 'When the green flag clicked' block. This means that when the green flag button is clicked the script will start.
* Now, let's write a simple script. We click on 'Control' to select 'forever' block, and consequently on 'Motion' to select 'set y to 0' block. Then, either under 'Sensing' or 'More Blocks' we have to select 'slider sensor value'. This allows us to control the character's vertical position with the slider sensor.

![Scratch Picoboard slider script]({{ base.url }}/public/images/picoboard/scratch_Picoboard_Recipe_Slider1.png)

* Checking the box next to 'slider sensor value' under 'Sensing' or 'More Blocks', or 'y position' under 'Motion' makes a sensor watcher appear on the stage, which allows us to see what value the slider sensor is reading. Move the slider on the PicoBoard and watch the readings change.
* Now let's try to use the slider to move the character up and down. If we want to move the character horizontally (left to right), instead of 'set y to 0' we have to select 'set x to 0' block.

![Scratch Picoboard slider script]({{ base.url }}/public/images/picoboard/Scratch_Picoboard_Recipe1.png)

* Now you can easily use the PicoBoard to control a character in your favourite video game.

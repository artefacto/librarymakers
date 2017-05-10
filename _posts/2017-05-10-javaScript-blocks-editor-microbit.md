---
layout: post
title: Getting started with JavaScript Blocks Editor (PXT) on Micro:Bit
categories: [recipes]
thumb: microbit-thumb.png
tags: [microbit, learnToCode, javascript]
author: Artefacto
---

## Intro

JavaScript Blocks Editor (PXT) is a drag and drop editor for JavaScript available on the Micro:Bit.

JavaScript Blocks Editor (PXT) is an updated version of the Javascript Blocks environment on the Micro:bit and includes some additional features like peer-to-peer radio.

In this tutorial, we're going to run and initial hello World script on our Micro:bit and also test out the hidden easter egg.

<!--more-->
## What you need

- Micro:bit and USB cable

## How
To open PXT, go to [Microbit.org](https://www.microbit.org/) and click on ‘Let's Code’ and then select _Let's Code_ from the JavaScript Blocks Editor (PXT) section.

(or you can go directly to [pxt.microbit.org/](https://pxt.microbit.org/))


![Microbit main screen]({{ base.url }}/assets/img/blog/microbit/select-PXT.png)

Like other code editors on the MicroBit it comes with an introductory tutorial to help you get started.

Click on 'Getting Started' to view the PXT Tutorial.

We're going to create a simple 'Hello World!' demo to check that everything is working.

Our code blocks in this example can all be found in the 'Basic' category.

First, let's add a On Start block. Anything within this block with run when the micro:bit is first connected or powered on.

![Microbit main screen]({{ base.url }}/assets/img/blog/microbit/hello-world.png)


Now, let's also add a _Forever_ block. This code will run until the device is switched off.

We can add a Show Icon block like this:

![Microbit main screen]({{ base.url }}/assets/img/blog/microbit/show-icon.png)


Now, save your code and upload it to your Mirco:bit board.

![Microbit main screen]({{ base.url }}/assets/img/blog/microbit/Hello-World-plus.png)


You should now see the "Hello, World!" text flash across the LED screen followed by the heart icon. The heart icon will say visible until we switch off the micro:bit or upload our next programme.

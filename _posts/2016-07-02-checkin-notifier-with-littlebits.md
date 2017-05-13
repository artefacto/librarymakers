---
layout: post
title: Create a check-in point with littleBits
categories: [recipes]
tags: [littlebits, CloudBit, electronics]
---

## Intro
Cloudbit is a LittleBits module that let’s you connect your LittleBits circuit with web services. This can be done via IFTTT, via the Cloud Control App or via the LittleBits API. Using IFTTT, you can connect to the CloutBit to control services like Twitter and Google Drive without needing to write any code.


![Cloudbit]({{ base.url }}/assets/img/blog/littlebits/cloudbit1.jpg)

In this example, we're going to create a notification checkin that will let people check-in at a particular location using CloudBit and IFTTT. When someone checks-in at the CloudBit location, you'll receive an email notification.

## What you need

- LittleBits CloudBit Kit and pressure sensor module.
- IFTTT Account

### How

If this is the first time you have used your CloudBit, you need to first connect it to your wifi network via the Cloud Control. Go to the Cloud Control at [http://control.littlebitscloud.cc](http://control.littlebitscloud.cc/) and follow the instructions to connect to your network.

To test whether your CloudBit is correctly connected to the network, you need to set up a basic circuit. Put together the circuit by connecting the LittleBit power module (USB connected to the wall) to the CloudBit connector module. Connect this to a light output.

Your basic CloudBit circuit should look like this:


![Cloudbit circuit]({{ base.url }}/assets/img/blog/littlebits/cloudbit-circuit.png)

Log in to IFTTT and click on create recipe

![IFTTT create a recipe]({{ base.url }}/assets/img/blog/littlebits/IFTTT-create-a-recipe.png)

First, we need to add a data source. This is the *'this'* in the ifthisthenthat recipe.

Click on this and search for 'Littlebits' and connect to the channel.

![IFTTT create a recipe]({{ base.url }}/assets/img/blog/littlebits/LittleBits-Trigger-Channel.png)

In the next step, select your CloudBit module from the dropdown list and click the **Create Trigger** button.

Now, click **that** to set the action for your recipe.

We want it to trigger when our module is on. We're using the Pressure sensor module so this will be when someone touches the pressure sensor.

Our notification can be sent by SMS, email or push notification. This can depend on the type of phone you use or how you'd like to receive notifications. In this case, we'll use the gMail notifier action.


![IFTTT create a recipe]({{ base.url }}/assets/img/blog/littlebits/LittleBits-gmail-action-channels.png)

Now, complete the action fields by setting the text of your notification. Make sure it's something meaningful. e.g. '{{DeviceName}}' someone is waiting at myLocation.

Give your recipe a name and click 'Create Recipe'.

![IFTTT create a recipe]({{ base.url }}/assets/img/blog/littlebits/LittleBits-Trigger-Recipe-Create.png)

Now you can create a LittleBits circuit with a touch sensor and put it at your check-in point. Add a sign for your check-in device to make it nice and clear.

When someone touches the sensor, you will be notified by email.

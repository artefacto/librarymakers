---
layout: post
title: Create a calendar notifier with littleBits
categories: [recipes]
tags: [littlebits, CloudBit, electronics]
---

## Intro
Cloudbit is a LittleBits module that let’s you connect your LittleBits circuit with web services. This can be done via IFTTT, via the Cloud Control App or via the LittleBits API. Using IFTTT, you can connect to the CloutBit to control services like Twitter and Google Drive without needing to write any code.


![Cloudbit]({{ base.url }}/assets/img/blog/littlebits/cloudbit1.jpg)


IFTTT (If This Then That) is a service that lets you connect to web apps and services to automate processes using simple conditional statements in the format If This Than That. The ‘If This’ part of the recipe is the trigger while (…Then That.) is the response. These statements are collated as ‘recipes’ that you can share and reuse.

IFTTT to make it super easy to control web applications like Facebook, Twitter or Google Drive, or communicate via SMS and Gmail- all without writing a single line of code.

## What you need

- LittleBits CloudBit Kit
- IFTTT Account
- Google Calendar or Office 360 Calendar

### How

If this is the first time you have used your CloudBit, you need to first connect it to your wifi network via the Cloud Control. Go to the Cloud Control at [http://control.littlebitscloud.cc](http://control.littlebitscloud.cc/) and follow the instructions to connect to your network.

To test whether your CloudBit is correctly connected to the network, you need to set up a basic circuit. Put together the circuit by connecting the LittleBit power module (USB connected to the wall) to the CloudBit connector module. Connect this to a light output.

Your basic CloudBit circuit should look like this:


![Cloudbit circuit]({{ base.url }}/assets/img/blog/littlebits/cloudbit-circuit.png)

Log in to IFTTT and click on create recipe

![IFTTT create a recipe]({{ base.url }}/assets/img/blog/littlebits/IFTTT-create-a-recipe.png)

First, we need to add a data source. This is the *'this'* in the ifthisthenthat recipe.

Click on **this** and search for 'Calendar'. You should get the option to connect the Google Calendar, Kyber or Office 365.

Select the Calendar channel you want to connect with.

If this is your first time connecting this Channel, IFTTT will request permission to access your calendar data. You need to approve this to continue.

Once you've connected the channel, you need to select what type of trigger you want to use. This is what sends the signal for your recipe to fire and can be the beginning of an event, a new calendar appointment added or based on the start of events matching a particular keyword.

In this example we're going to set the trigger to be when a new event is added to our calendar.


![IFTTT set a calendar trigger]({{ base.url }}/assets/img/blog/littlebits/Choose-a-calendar-trigger-annotated.png)

Because there's no additional fields to set for this trigger, we can just click **Create Trigger** to skip step 3 of our recipe setup.

It's now time to set the follow up action for our recipe. The *that* of the equation.

![IFTTT set a calendar output]({{ base.url }}/assets/img/blog/littlebits/IFTTT-create-recipe-that.png)

Click on **that** and search for the LittleBits Action channel. Clicking on the LittleBits channel gives you three options for your action.

![IFTTT set a calendar trigger]({{ base.url }}/assets/img/blog/littlebits/LittleBits-Action-Options-annotated.png)

The *Activate Output* option activates your LittleBits module output for 3 seconds while the *Deactivate Output* option will basically switch off the output of your module.

The *Set Output* option gives us a few more options to work with so we are going to _select this one_.

You need to select your CloudBit module from the dropdown list. This is the name you gave your CloudBit when you first set it up.

Next, set the output level. As we're using an LED, we can set the output to 100%.

And we want the duration of the notification light to be long enough for us to notice it, so we can set this to 15 seconds.

Once your action is set, you can click the **Create Action** button.

Now, give your recipe a meaningful name and click **Create Recipe**.


![IFTTT Calendar LittleBits recipe]({{ base.url }}/assets/img/blog/littlebits/IFTTT-cloudbit-calendar-recipe.png)

You'll then be redirected to the recipe page where you can test it out by clicking on 'Check Now'. You can also view the recipe log to make sure everything is running ok.

![IFTTT recipe options]({{ base.url }}/assets/img/blog/littlebits/recipe-options-annotated.png)

If your recipe is running ok, add a new event to your calendar and watch your LED light turn on to notify you.

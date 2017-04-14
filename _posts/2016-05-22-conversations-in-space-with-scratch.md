---
layout: post
title: Create a conversation with Scratch
categories: [recipes]
tags: [scratch, creative-computing]
---

## Intro

With Scratch, you can create simple stories using different characters. In this example, we will create a simple conversation between two characters.

 If you're not familiar with the Scratch editor interface, see [this intro](/the-scratch-user-interface).

 This is what we are building (though this is just an outline that you can create your own story from)

![Conversation in space]({{ base.url }}/public/images/scratch/7tedYo0Z6q.gif)

## How
The first thing to do is to choose your 'Sprite'. To remove the default Sprite (Scratch cat), right-click on the sprite icon and choose 'Delete'.

![Delete the Scratch sprite]({{ base.url }}/public/images/scratch/delete-cat-sprite.png)

You can then add a new sprite from the sprite gallery.

![Add a new sprite]({{ base.url }}/public/images/scratch/sprite-library.png)

We can add a backdrop to help set the scene for our conversation to take place. Click on the 'New backdrop' option and choose where you'd like to set your story.

![Add a new backdrop]({{ base.url }}/public/images/scratch/add-a-backdrop.png)

Choose whatever backdrop you want for your library. For this example, we're going to use one of the Space backdrops.

![Backdrop library]({{ base.url }}/public/images/scratch/backdrop-library-space.png)

Now, let's add our first conversation script.

We start with a 'When Flag Clicked' block. It looks like this and you can find it under the Events category:

![When flag clicked]({{ base.url }}/public/images/scratch/when-flag-clicked-block.png)

This means the script will start running when we click the green flag icon that appears at the top of the stage.  

![Run the script]({{ base.url }}/public/images/scratch/run-the-script.png)

Then add a dialogue block. It's found in the Movement palette. You can add whatever greeting you want here.

Next add a *wait block*. This gives the pause in the conversation where another character can reply.

Your script should now look like this:

![First conversation block]({{ base.url }}/public/images/scratch/conversation-part-1.png)

Let's add a second character for our robot character to talk to.  As before, add a new Sprite from the sprite library. Select the new sprite and add a script that continues the conversation.

![Second conversation block]({{ base.url }}/public/images/scratch/conversation-part-2-reply.png)

The conversation exchange is all about timings. Make sure that each character is given time to say something and hear the reply.

You can see that the length of time the first character is speaking and the time the second character waits match.

You can add additional *wait and say* blocks to keep the conversation going.

Our first character's script looks like this:

![Character 1 script]({{ base.url }}/public/images/scratch/character-1-full-script.png)

And the second character's script looks like this:

![Character 2 script]({{ base.url }}/public/images/scratch/character-2-full-script.png)

You can extend the story further with additional sprites and backdrops.

![Spaceship]({{ base.url }}/public/images/scratch/spaceship.png)

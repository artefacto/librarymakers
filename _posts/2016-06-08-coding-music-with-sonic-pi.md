---
layout: post
title: Coding your first music with Sonic Pi
categories: [recipes]
tags: [raspberrypi, music, coding, sonicpi]
---

## Intro
Here, we're going to write our very first Sonic Pi program. This will cover the basics of coding with Sonic Pi, but if you haven't used it before you can check out the [introductory guide here](/getting-started-with-sonic-pi).

## Coding with Sonic Pi

The most basic code you can write with Sonic Pi is play followed by a number. The number represents the musical pitch, lower numbers make lower pitched beep and higher numbers make higher pitched beep sound.

    play 75

The notes are based on the notes on a piano (it uses MIDI keyboard numbers). So, if you type *play 60*, you are telling the program to play the 60th note on the piano.

You can use the sleep option (followed by the duration) to add a break between notes. For example:

    play 60
    sleep 0.5
    play 62
    sleep 0.5
    play 64
    sleep 0.5
    play 60
    sleep 0.5


  This combination will play everyone’s favourite tune, *Frère Jacques*.

But you don’t have to use the MIDI numbers if you know the notes. You can use notes in Sonic-Pi too.

    play :C
    sleep 0.5
    play :D
    sleep 0.5
    play :E
    sleep 0.5
    play :C
    sleep 0.5  

 If we want to play it through more than once , we wrap it in a loop specifying how many times to run the program using `do` and `end`.

     2.times do
      play 60
      sleep 0.5
      play 62
      sleep 0.5
      play 64
      sleep 0.5
      play 60
      sleep 0.5
    end

If we want to keep repeating a particular piece of music, use a forever loop:

    loop do
      play 60
      sleep 0.5
    end

You can specify the synth to use to change the sound.

    use_synth :fm
     2.times do
      play 60
      sleep 0.5
      play 67
      sleep 0.5
    end

The synth options (like other code in Sonic Pi) will autocomplete so you can try out different ones at random or you can refer to the list of available synths from the help panel at the bottom of the screen.    

![Sonic Pi synth options]({{ base.url }}/public/images/sonic-pi/synth-options.png)


And you can add samples. Select samples on the left hand side of the help window to browse through the samples and how they can be used.

    2.times do
     sample :loop_amen
     sleep 1.753
    end

Let’s add a backbeat (because everything is better with a backbeat).

To play more than one thing at a time, you can wrap your code together using **threads**.    

    # Frère Jacques again - this is a comment in
    # the code, they always start with a # symbol

    thread do
     use_synth :beep
     loop do
      sample :drum_cymbal_closed
      play 60
      sleep 0.5
      play 62
      sleep 0.5
      play 64
      sleep 0.5
      play 60
      sleep 0.5
     end
    end

And what about if you are still creating and you want to change things as you go? You can use **live_loops** to create music on the fly. Change the sample and click *Run* again to hear the new version instantly.

You need to give your *live loop* a name, something descriptive so you can keep track of what it is. Ours is called breakbeat_backbeat.

    live_loop :breakbeat_backbeat do
      sample :loop_breakbeat
      sleep 2
    end

You can use lots of live_loops at a time to play different samples, beats and notes simultaneously.

There are lots of options and additional functionality to discover with Sonic Pi but this is enough to get you started coding your very own music.

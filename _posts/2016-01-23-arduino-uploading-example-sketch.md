---
layout: post
title: Uploading your first sketch on Arduino
categories: [recipes]
tags: [arduino, sketches, IDE]
---

## Intro
To interact with an Arduino board (such as the Uno), you need to use the Arduino Integrated Development Environment (IDE). This can be downloaded from: [https://www.arduino.cc/en/Main/Software](https://www.arduino.cc/en/Main/Software)

The Arduino hardware runs programs called ‘sketches’ (written in the C++ language) that are uploaded to it. Using the IDE, you can run example sketches, modify existing sketches or create your own.

In this tutorial, we’re using an Arduino Uno so you’ll need to update the references to that to match the Arduino model you’re using.

## What you need

- An Arduino Board
- Arduino IDE software


## How

- **Connect the Uno to your computer** with a USB cable. Once it’s correctly connected, the green LED (labelled PWR) should light up.

- You need to **tell the IDE what Arduino board you are using***. From the Tools menu, go to Board and then select the option that matches your Arduino board.

- You also need to **set the serial port** - the serial device of the Arduino board you are using. Again, from the Tools menu, now go to Serial Port and choose  /dev/tty.usbmodem (this may vary, for older boards you may need to use /dev/tty.usbserial).

If you’re not sure which Serial Port option to choose, disconnect the Arduino from your computer. It’s Serial Port will then disappear from the options. Reconnect and select the relevant serial device from the list.

The IDE should now be able to communicate with your Arduino board.

- To **upload the sketch**, choose one of the options from the examples menu (e.g. File > Examples >01.Basics > Blink)


- Click the "Upload" button in the environment.

![Arduino IDE menu]({{ base.url }}/assets/img/blog/arduino-IDE-menu.png)


- The lights on the board will blink while the sketch is being uploaded. If the upload was successful,  you will see the orange pin 13 (L) LED start to blink (in orange). and the message "Done uploading" will appear in the status bar.


![Upload to arduino board]({{ base.url }}/assets/img/blog/arduino-upload-blink-sketch.png)


Congratulations, you have successfully run a program on your Arduino board.



## More info

About the Arduino IDE
[https://www.arduino.cc/en/Guide/Environment](https://www.arduino.cc/en/Guide/Environment)

Other projects to try
[https://www.arduino.cc/en/Main/ArduinoStarterKit
](https://www.arduino.cc/en/Main/ArduinoStarterKit)

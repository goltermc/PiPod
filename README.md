# PiPod
Code to make a Raspberry Pi appear as an iPod to my car radio
This project started out as an application for the Beaglebone Black clled beaglepod.
I found it while poking around on the web.

Sometime ago I obtained a vehicle with a "radio" which would talk to an iPod.
Not wishing to spend money on an iPod, I pursued creating my own "iPod".
I started searching for the protocol used to communicate with an iPod.
I found a web page which discusses the Apple Appliance Protocol at https://nuxx.net/wiki/Apple_Accessory_Protocol
Since these things tend to disappear over time, a copy of that page is stored herein under AAP_HTM. You should be able to view it in a browser.
Along the way , I found numereous anrdoid apps which would make an android device "look" like an ipod.
None of these had any reasonable documentation. I was frustruated.
Then I stumbled on beaglepod. It is written entirely in c/c++, which I've used for many years.
I tried to get this to compie on the beaglebone black but kept running into library issues.
Finally, I moved the source to a spare raspberry pi and was able to get it to compile completely.

I've spent a good deal of effort, getting things set up.
At this writing , I have many of the tests working but have not yet connected anything to the radio.

The connection is intended to come from the raspberry pi's serial port via an adafruit serial to usb adaptor
to the radio's usb input ( which will also power the raspberry pi).

The adafruit adaptor I used can be found here https://www.adafruit.com/product/954.
I attached it to the raspberry pi using directions found here https://learn.adafruit.com/adafruits-raspberry-pi-lesson-5-using-a-console-cable
Other serial to usb adaptors might work. You will have to adapt the code to use something else.

It connected to my mac first try. At this writing I am still attempting to get all the tests running.
I'll update this file as success warrants.

Under the test directory is a "very" truncated iTunes library.
It contains three mp3 files I found on the web which are not copyrighted.

I have no intent of playing anything other than music. Not interested in video. Feel free to extend this if you like.

This project is copyrighted under the GNU Gpl 2 license.

All sources retain the original copyright notice with the name of the original author.

Aside from a little formatting and cleanup, I've made few changes. I also made a few changes to Makefile.ac.

Eventually, I'll create instructions for building on the raspberry pi, including all the libraries which must be loaded to make this work.

Use this as you like I make no warantees whatsoever.



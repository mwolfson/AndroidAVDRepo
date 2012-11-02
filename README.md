AndroidAVDRepo
==============

A collection of pre-configured Android emulator images.

What this is for:
-----------------

This repo is designed to allow Android developers to download pre-configured configurations files (in the form of an ini file, and an avd folder).  These files contain the configuration parameters for common Android devices, and can be used with the emulator from the Android Developer Tools (ADT).  The intent is to save time configuring devices, and also to have a way to quickly recover a clean emulator image if something becomes corrupt or stops working as expected.  

Naming the emulator instances:
------------------------------

The images are named to contain 4 important pieces of information:
* The name the device was marketed as in the US
* Phone or Tablet
* The Android Version Number it is configured with
* The screen resolution (ldpi, mdpi, hdpi, xhdpi)

For instance G1_phone_16_ldpi is for the following device:  HTC G1, which is a phone that runs version 1.6 of Android and has a low-resolution display (ldpi)

Options enabled:
----------------

The emulators have all been configured with:
* Snapshots (if they are running a pre-4.0 release of Android)
* HAXM Hardware Acceleration (if they are running post ICS)
* They all have keyboard support enabled

How to Use:
===========

Find the .android folder on your system (this is where the emulator AVD files are stored).  It will most likely be in your home directory (ie. /home/user/.android)

In that folder is the avd folder, cd into that.

Clone the repo into this folder (make sure to include the . at the end of the command) so the files are placed directly into this folder:
`git clone https://github.com/mwolfson/AndroidAVDRepo.git .`

So it will look something like this:
`/Users/youruserid/.android/avd/git clone https://github.com/mwolfson/AndroidAVDRepo.git .`

That's it.  Next time you start your avd manager you will see these new emulator instances in your list of available devices.  You can then modify the AVDs to your specific requirements.

Plans
=====
I hope to create a lot more AVD images, to contain as many different devices in this repo as possible (pull request are welcome!).

Android Virtual Devices Repository
==============

This repo is a collection of pre-configured Android emulator configuration files (AVD and ini files) and definitions (in devices.xml file).

# Setup

Android emulator expects that everything will be in your .android directory under your $HOME folder.  Device ini files point to the full path of the avd directory for each device, including the $HOME directory of the user that created the device.

To get around issues with those links and the need to move or copy things around, a script called 'linkavd' has been created.

Every time you pull down new AVDs from the repo, run linkavd from the checkout directory and it will create the proper ini files. The path in the ini file will point to the avds in your repo, and the ini files will be linked to from your '$HOME/.android' directory so that they are available for your use.  The script will also run an update command, which repairs something or other automagically, so the path changes don't make the AVDs unusable :)


## Smartphones

- Nexus One, by Google
- Nexus S, by Google
- Galaxy Nexus, by Google
- Nexus 4, by Google
- G1 aka Dream, by HTC
- Droid (original), by Motorola
- Droid X, by Motorola
- Droid Razr Maxx HD, by Motorola
- Galaxy S2, by Samsung
- Galaxy S3, by Samsung
- Galaxy S4, by Samsung


## Tablets 

- Kindle Fire, by Amazon
- Kindle Fire HD (7" and 8.9"), by Amazon
- Galaxy Tablet, by Samsung


# Growing the collection

Feel free to fork, clone and git-push to increase the number of devices defined.

Thanks to [Mike Wolfson](https://github.com/mwolfson/AndroidAVDRepo) and [Luxurious Animals](https://github.com/luxuriousanimals/AndroidAVDRepo) for the original idea and some AVDs!
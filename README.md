Android Virtual Devices Repository
==============

This repo is a collection of pre-configured Android emulator configuration files (AVD and ini files) and definitions (in devices.xml file).

Specifically, these are intended to assist web developers with testing websites across a multitude of versions of Androids with different device configurations.  As such they usually include a hardware keyboard and buttons even when the device does not actually include those features.

If you feel strongly about not including these convenience features, let me know and maybe we can figure something better out.

# Setup

Because of the way that the Android tools expect things to be configured, you must run the "linkavd" script every time that you pull from the repo.  The tool will hard link the AVDs from this repo into your ~/.android folder and create and link the .ini files for those AVDs from ~/.android/avd/*.ini to the ini directory here.

If you are not using a system compatible with bash, copy all of the files under "avd" to the directory where your AVDs are installed.  Search and replace "/Users/user/.android/" in the .ini files with the correct path.


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

## HAXM

For performance purposes, where the API supports it (2.3+), an alternate Intel Atom-based device has been configured.  These devices have i or -i at the end.  Using one of these devices requires that you have Intel HAXM installed.

http://software.intel.com/en-us/articles/intel-hardware-accelerated-execution-manager


# Growing the collection

Feel free to fork, clone and git-push to increase the number of devices defined.

Thanks to [Mike Wolfson](https://github.com/mwolfson/AndroidAVDRepo) and [Luxurious Animals](https://github.com/luxuriousanimals/AndroidAVDRepo) for the original idea and some AVDs!
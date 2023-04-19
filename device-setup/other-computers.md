# Regular computers

On regular machines the process is similar to formatting any computer. It's done through flashing a usb drive and getting it to boot through keyboard commands.

**Recomended devices:**

* [Zimaboard 432](https://shop.zimaboard.com/products/zimaboard-single-board-server-for-creators-8g-32gb-linux-windows-openwrt-pfsense-andorid-libreelec-development-board-low-cost-hackable-single-board-server)

#### Needed hardware

* Any spare computer with a storage that you can format, like old desktop or laptop machines with a hard-drive or ssd with at least 30Gb of storage
* Any USB drive with at least 2Gbs of storage
* Internet connection through ethernet cable
* Keyboard
* Monitor and cables

#### Needed software

* Image burner, recommended: [Balena Etcher](https://www.balena.io/etcher/)

#### Preparing USB flash drive

Download and use the **Generic x86\_64 (GPT)** image for regular amd machines at: [http://releases.earthdefenderstoolkit.com](http://releases.earthdefenderstoolkit.com/)

Use the image burner to burn the image to the usb flash drive.

#### Installing the Offline Toolkit

* Insert the flashed USB into the computer
* Insert the ethernet cable with Internet coming from your router into the computer
* Discover how to trigger boot menu or how to enter BIOs and ajusting booting order
* Select boot to happen throgh UEFI or USB, and the device should start setup
* Setup can take several minutes depending on the computer's capabilities&#x20;
* Check the [Balena Dashboard](https://dashboard.balena-cloud.com/) for the device to come online, or check if a new WiFi hotspos has appeared
* In case a long time has passed without anything happening, unplug and re-plug power supply

In case you have problems with your setup, check the [troubleshooting.md](troubleshooting.md "mention") section. If everything worked, check [syncing-content.md](../device-usage/first-steps/syncing-content.md "mention") to get content into your new Offline Toolkit.




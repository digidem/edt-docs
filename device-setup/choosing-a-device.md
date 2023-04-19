# Choosing a device

There are a multitude of different boards that can be used to run EDT Offline. From recycled hardware, such as old computers to tiny, low-power single-board-computers.

<img src="../.gitbook/assets/pi4_rockpi_zima (1).jpg" alt="" data-size="original"> Raspberry Pi 4, Rock Pi 4, ZimaBoard

Some important things to pay attention when choosing the right device:

* Ease to setup (single-board-computers are always easier)
* Price, including power supply, storage, case, etc.
* WiFi range and capacity
* Energy usage
* Power
* Availability
* Form factor

#### Easiest to setup, but more expensive and less CPU and WiFi power

![Rock Pi 4 with casing](https://cdn.shopify.com/s/files/1/0248/6557/0909/products/DSC01592\_900x600.jpg?v=1636979793)

Single-board-computers are the easiest to setup. We’ve tested on the Raspberry Pi 4 and Rock Pi 4, and had great results. The Raspberry 3 should be able to handle as well, but we haven’t tested yet.

For all these boards it's a question of downloading the latest release from the [Github repository](https://github.com/digidem/edt-offline/releases/latest), and burning them to an class 10 micr-sdcard using a software such as [Balena Etcher](https://www.balena.io/etcher).

**Recommended: Rock Pi 4 B+**

We recommend the [**Rock Pi 4 B+**](https://rockpi.org/rockpi4) board because of the chip shortages around the globe resulting in a scarcity of the Raspberry Pi boards.

Besides the board itself you’ll need some cooling, as the boards tend to overheat without appropriate cooling system.

You’ll also need a power supply in case it isn’t included with the board, and it’s important that it’s a USB C 5v with at least 3A.

And finally you’ll need a storage, which should be at least class 10 micro-sd card.

**Buying from Amazon:**

* [Rock Pi 4B](https://www.amazon.com/dp/B0B4MWBKR7?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [3.5A USB C power supply](https://www.amazon.com/dp/B07TYQRXTK?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [32GB Class 10 Micro SD card](https://www.amazon.com/dp/B07XDCZ9J3?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [Case with built-in heatsink](https://www.amazon.com/dp/B0B7P41CTS?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)

#### Cheap, powerful CPU and WiFi, but harder to setup

![Zimaboard with PCI express Wifi module](<../.gitbook/assets/zimaboard\_wifi (1).jpg>)

Any old desktop of notebook can serve as an EDT Offline device, but they’re a bit harder to setup, and they usually require entering the computer’s BIOS and change some settings to set USB as primary device to boot from. That will require are least a key board and a screen, and appropriate cables to connect to it.

After changing the BIOS settings, you’ll need to burn the amd64 image from the [release page](https://github.com/digidem/edt-offline/releases/latest), and burn it to a thumb drive with enough storage.

Turn the device off, insert the thumb drive, and turn it back on. This process can take minutes and might require a few restarts, but once finished will have a fully working EDT Offline instance.

If you’re buying a computer to use with EDT Offline, we recommend mini-pcs such as the [Intel Nuc](https://www.intel.com.br/content/www/br/pt/products/details/nuc.html).

**Recommended:** [**ZimaBoard**](https://www.zimaboard.com/)

It’s one of the cheapest boards you can get, with the smallest form-factor. It’s PCI express port makes it easy to plug different WiFi adapters, which will depend on how fast you want the connection to be, how many people it can handle at the same time and how far you need your WiFi hotspot to go.

**Buying from Amazon**

* [ZimaBoard](https://www.amazon.com/dp/B0BKL4SRJT?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [PCIe WiFi Adapter](https://www.amazon.com/dp/B08J8BHBXJ?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [Mini Display to HDMI Adapter](https://www.amazon.com/dp/B0134V3KIA?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)

### Full list of potential devices

#### Single Board Computers

Because they usually use ARM cpus they tend to be consume less energy and have a smaller form-factor, but are less capable, and don't usually include storage, casing or a cooling system

* [Rock Pi 4](https://a.co/d/95OOIZM) (\~90 USD) 🇺🇸
  * 4GB LPDDR4
  * RK3399 Hexa-Core
  * Gigabit Ethernet
  * Dual-Band WiFi
* [Raspberry Pi 4](https://a.co/d/iAgYwIs) (\~125 USD - \~152 USD) 🇺🇸
  * 1GB / 2GB / 4GB / 8GB LPDDR4
  * BCM2711 Quad-Core
  * Gigabit Ethernet
  * Dual-Band WiFi
* [reRouter CM4 1432](https://www.seeedstudio.com/Dual-GbE-Carrier-Board-with-4GB-RAM-32GB-eMMC-RPi-CM4-Case-p-5029.html) (\~160 USD) 🇨🇳
  * Includes casing & power supply
  * 4GB LPDDR4
  * 32GB eMMC
  * BCM2711 Quad-Core
  * 2x Gigabit Ethernet
  * Dual-Band WiFi
* [RockPro 64](https://pine64.com/product/rockpro64-4gb-single-board-computer/) (\~80 USD) 🇨🇳
  * 4GB LPDDR4
  * RK3399 Hexa-Core
  * Gigabit Ethernet
  * No WiFi included
* [ZimaBoard](https://www.seeedstudio.com/ZimaBoard-216-X86-p-5298.html) (\~120 USD - \~200 USD) 🇺🇸
  * Includes casing & power supply
  * 16GB / 32GB eMMC
  * 4GB / 8GB LPDDR4
  * Intel Celeron N3350
  * 2x Gigabit Ethernet
  * No Wifi, but 4x PCIe ports for dongle
* [ODYSSEY-X86](https://www.seeedstudio.com/ODYSSEY-X86J4125800-p-4915.html) (\~220 USD - \~300 USD) 🇨🇳
  * 0 / 64GB / 128GB eMMC
  * 8GB LPDDR4
  * Intel Celeron J4125
  * 2x Gigabit Ethernet
  * Dual-Band WiFi
  * 2x M.2 PCIe
*   [Khadas VIM2](https://a.co/d/0d0TWcv) (\~89 USD - \~100 USD) 🇺🇸

    > Not confirmed Balena support

    * 16GB / 32GB eMMC
    * 2GB / 3GB LPDDR4
    * Amlogic S912 1.5 GHz 64Bit Octa Core ARM Cortex-A53 750MHz
    * Gigabit Ethernet
    * Dual-Band WiFi MIMO 🔥

#### Fanless Mini PCs

These tend to be cheaper and more powerful then SBCs, and come complete with storage, casing and power supply

* [Bmax B1 Plus](https://www.amazon.com/Bmax-B1-Plus-Computer-Ethernet/dp/B0BHP34TH1/ref=sr\_1\_4?keywords=Bmax%2BMini%2BPC\&qid=1677967510\&s=electronics\&sr=1-4\&ufe=app\_do%3Aamzn1.fos.f5122f16-c3e8-4386-bf32-63e904010ad0\&th=1) (\~120 USD) 🇺🇸
  * 8GB DDR3
  * 128GB SSD
  * Intel Celeron
  * Gigabit Ethernet
  * Dual-Band WiFi
* [N40](https://a.co/d/5QoK6Uw) (\~110 USD) 🇺🇸
  * 4GB DDR4
  * 64GB eMMC
  * Intel Celeron
  * Gigabit Ethernet
  * Dual-Band WiFi
* [Beelink T4 Pro](https://a.co/d/9OSdXs4) (\~100 USD) 🇺🇸
  * 4GB DDR
  * 64GB eMMC
  * Intel Celeron
  * Gigabit Ethernet
  * Dual-Band WiFi
* [MeLE Quieter2Q](https://a.co/d/8EMGSYe) (180 USD - 280 USD) 🇺🇸
  * 4GB - 8GB LPDDR4
  * 64GB - 512GB M.2 SSD
  * Intel Celeron
  * Gigabit Ethernet
  * Dual-Band WiFi
* [AWOW](https://a.co/d/f6pVMX6) (\~130 USD) 🇺🇸
  * 4GB DDR4
  * 64GB eMMC
  * Intel Celeron
  * Gigabit Ethernet
  * Dual-Band WiFi

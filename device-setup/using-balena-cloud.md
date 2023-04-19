# Using Balena Cloud



> &#x20;Third party company will be managing a monitoring platform for your devices, and they have backdoors to your devices

You'll need some software to burn images to a storage device (pen drive or sd card), we recommend [Balena Etcher](https://www.balena.io/etcher/).

Anyone can deploy there own EDT-Offline by following these steps:

1. Click on "[Deploy with Balena](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/digidem/edt-offline)”
2. You'll be asked to create a Balena Cloud account
3. You'll be prompted to deploy a new fleet, change the name if necessary and click on "create and deploy”
4. Click on the "Add device” button
5. Leave in "Production" mode unless you'd like to experiment and have ssh access to the device
6. To setup the device you'll need Internet, choose the way you intend to connect, either through WiFi (provide the credentials) or Ethernet cable
7. Finally either click "Flash" which will automatically flash using Etcher, or using the arrow click on "Download balenaOS", which will download the image file
8. Insert the storage in the computer and burn the image
9. Finally insert the storage to the device and watch your [Balena Cloud Dashboard](https://dashboard.balena-cloud.com), a new device should appear and start updating it's software
10. To sync with default content you'll need to get in touch with us through e-mail, Telegram or Whatsapp

> &#x20;Change your device location on the Balena Cloud “Location” tab. This is recommended if you don’t want your device to be found on the [Balena Hub](https://hub.balena.io).

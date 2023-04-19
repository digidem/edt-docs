---
description: What are the basic technical skills needed for this setup?
---

# Introduction

> ⚠️ Beware that during Beta we're relying on the service Balena Cloud by a company, and they have back doors to all devices.&#x20;

The process for preparing a device to run Earth Defenders Offline Toolkit requires a notebook or desktop computer, used to "burn" images to sd cards or usb flash drives. So basic skills on using them is required.

For help with common technical issues, see the [faq.md](../overview/introduction/faq.md "mention") section of this guide. For additional support, please check out the community of active users and maintainers of the Earth Defenders Toolkit on our public [Discord](https://discord.gg/ZDPWMyQP), [Telegram](https://t.me/+3t9fPkrkg4oxNjU5) group and [online forum](https://forum.earthdefenderstoolkit.com/).

### Different processes

Any old computer can be recycled to run the Earth Defenders Offline Toolkit software stack. Ideally you should format old machines to run our light Operating System, see [other-computers.md](other-computers.md "mention").

The Offline Toolkit can also run the services alongside your existing Operating System see [using-docker.md](using-docker.md "mention"). This process is unsupported and disconnected from Balena Cloud, thus respects data sovereignty.

If the intention to purchase a new device for this purpose, we encourage buying a single-board-computer, as they tend to be cheaper, more mobile, uses less energy and are easier to setup, see [single-board-computers.md](single-board-computers.md "mention").

### Supported Installations

The Digital Democracy team will have access to the device and all data, but will not access or extract data without consent. We'll monitor devices for software and hardware problems, so we can provide support.

But the Balena company will also have backdoors into the device, which most probably won't be used, but **can** be used.

We currently generate supported ready-to-use images that can be flashed into any regular computer and selected single-board-computers.

To see all released support-mode images head to: [http://releases.earthdefenderstoolkit.com](http://releases.earthdefenderstoolkit.com/)

Continue to [choosing-a-device.md](choosing-a-device.md "mention") to find the best fit for your needs.

### Unsupported installations

The process is very similar to the supported one, but instead of downloading our image you'll create your own using Balena Cloud. Simply click [here](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/digidem/edt-offline) and Balena will walk you through the process.

You'll generate your own image, but running our software. That way you can manage your own fleet of devices.

Check [connecting-to-the-internet.md](../device-usage/first-steps/connecting-to-the-internet.md "mention") and [syncing-content.md](../device-usage/first-steps/syncing-content.md "mention") to learn how to get the content for your Offline Toolkit.

You'll still need to get in touch with us at least to authorize syncing the content, see [support.md](../support.md "mention").

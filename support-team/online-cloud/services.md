# Services

## Syncthing

A free, open-source peer-to-peer file synchronization application available for most plaforms. It can sync files between devices on a local network, or between remote devices over the Internet. Data security and data safety are built into the design of the software. It’s a FOSS alternative to [Resilio Sync](https://www.resilio.com).

The app is used for keeping up-to-date content (mapeo configs and tiles, offline websites, f-droid repository, etc) available for when community or organization devices go online.

The initial handshake between instance in the cloud and other devices is initialized automatically by the EDT Offline device, but needs to be accepted by someone with access to the Cloud service.

## File Browser

Provides a file managing interface within a specified directory and it can be used to upload, delete, preview, rename and edit files. It allows the creation of multiple users and each user can have its own directory. It can be used as a standalone app. It's a FOSS alternative to Google Drive, without the office suites.\*\*\*\*

It's used for browsing content both in the cloud as well as on the offline device. The team giving support to communities should use it to add or remove content that's hosted on the cloud. The offline devices can use it to share files back with the support team, or within the local network.

## F-Droid Repository

F-Droid is an app store and software repository for Android. Applications can be browsed, downloaded and installed from the client app without the need to register for an account. It's a FOSS alternative to the Google Play store.

We’ve forked a client app and created our own [EDT Apps](https://github.com/digidem/edt-apps) client, which comes with our own [EDT app repository](https://github.com/digidem/edt-fdroid-repository), as well as the repository that's running on the EDT Offline devices.

Regular F-Droid clients can also make use of the EDT repository by simply adding the url to their list of repositories or scanning the QR code presented.

## Secure Scuttlebut Room

The main client app, [Manyverse](https://www.manyver.se/), is a social network without the bad stuff, built on the peer-to-peer SSB protocol. It's free and open source, and available for desktop and mobile. It's not running in the cloud owned by a company, instead, all data lives entirely on user devices. This way, even when offline, users can scroll, read anything, and even write posts and like content. When the device is back online, it syncs the latest updates directly with other devices, through a shared local Wi-Fi or on the internet.

The SSB Room is a service that enables peers to “meet” online and exchange data. By running our own Room we can connect partners between themselves as well as support teams. It has user management features (allow- & denylisting + moderator & administrator roles), all administered via the web dashboard.

## Minio Storage

MinIO is a high performance object storage solution that provides an Amazon Web Services S3-compatible API and supports all core S3 features. It’s a FOSS alternative to Amazon S3.

It's used for organizing Terrastories data into buckets. That way if a partner wants to have it’s Terrastories published on the cloud, we can sync it’s Minio bucket, which is running on the EDT Offline device, and run a Terrastories instance on the cloud pulling from that data. It provides an organized way of maintaining online and offline Terrastories instances in sync.

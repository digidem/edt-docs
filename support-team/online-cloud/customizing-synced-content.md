# Customizing synced content

### 1. Web scrapping

The scrapping of websites is done by [browsertrix-crawler](https://github.com/webrecorder/browsertrix-crawler) command-line. Find more instructions in the [crawling documentation](https://www.notion.so/Web-Crawling-c8f980b0fac54cdc9c2d9a308461ddd9).

Some experimentation is needed to find best practices on how to get exactly the amount of pages we want scraped, and for each language.

The scrapping might take a long time. Use the output warcz files on the next step.

### 2. Upload to the Cloud

Navigate to the [FileBrowser service](https://files.earthdefenderstoolkit.com) on the EDT cloud.

<figure><img src="../../.gitbook/assets/Untitled.png" alt=""><figcaption></figcaption></figure>

There are different directories within the `content` directory, each for a content type: F-Droid repository data; Desktop installers; Mapeo data (configs and tiles); and Offline Websites.

Create a new folder for your new content if needed:

Make sure there’s enough left storage on the server, and to upload new content simply drag to the folder or use the upload icon to select the file from your computer:

<figure><img src="../../.gitbook/assets/Untitled 1 (1).png" alt=""><figcaption></figcaption></figure>

Once the new content is uploaded we can sync it to EDT devices.

### 3. Sync it

Navigate to the [Syncthing service](http://sync.earthdefenderstoolkit.com/) on the EDT cloud and follow the same steps as in [content-syncronization.md](../../device-usage/bundled-applications/content-syncronization.md "mention").

### 4. Adding to device

Check instructions on [syncing-content.md](../../device-usage/first-steps/syncing-content.md "mention")on how to start syncing with a new device. You'll how to get your Syncthing ID.

On the EDT Cloud instance search for that ID:



<figure><img src="../../.gitbook/assets/Untitled 6 (1).png" alt=""><figcaption></figcaption></figure>

Give the new device a descriptive name, and got to the **Sharing** page:

<figure><img src="../../.gitbook/assets/Untitled 7.png" alt=""><figcaption></figcaption></figure>

On the **Sharing** page select all the folders that are relevant for the new device, usually the defautls:

<figure><img src="../../.gitbook/assets/Untitled 8 (1).png" alt=""><figcaption></figcaption></figure>

On EDT Cloud you should see that the device is starting to sync:

<figure><img src="../../.gitbook/assets/Untitled 9.png" alt=""><figcaption></figcaption></figure>

On the local Offline Toolkit you should also see syncing happening with more details such as download rate, and amount synced so far.

You're done. Now every time the Cloud updates the content folder, the Offline Toolkit devices will automatically sync whenever they're online.

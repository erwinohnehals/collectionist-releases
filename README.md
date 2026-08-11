# Collectionist — releases

Installers for **Collectionist**, a local-first desktop collections manager.
This repository holds nothing else: no source, no issues, just the releases and
the `latest.json` every installed app reads on launch to find out whether a
newer version exists.

**[Download the latest release →](https://github.com/erwinohnehals/collectionist-releases/releases/latest)**

## What is in a release

| File                             | What it is                                                    |
| -------------------------------- | ------------------------------------------------------------- |
| `Collectionist_x.y.z_x64-setup.exe` | Windows installer (NSIS). This is the one to download.     |
| `Collectionist_x.y.z_x64_en-US.msi` | Windows installer (MSI), for deployment tooling.           |
| `*.nsis.zip` and `*.sig`         | The update package and its signature. The app downloads these itself; you never need them. |
| `latest.json`                    | What the in-app updater reads.                                |
| `collectionist-demo-library.zip` | Optional. A populated library to look around in — see below.  |

## Installing

Run the `.exe` and follow it. The installers are not code-signed yet, so
Windows SmartScreen will say **"Windows protected your PC"** on a first
install — click **More info**, then **Run anyway**. Updates applied from inside
the app do not show this again; they are verified by the app's own signature
instead.

## Starting with the demo library

`collectionist-demo-library.zip` is a ready-made collection — vintage
motorcycles and vintage cars, with photographs, timelines, invoices, saved
filters and a wish list — so there is something to look at before you have
typed anything in.

Install it **before the first launch**: unpack the zip into

```
%APPDATA%\com.collectionist.app
```

so that a `library` folder appears there. That is it. Launch the app and it is
already full.

To go back to an empty app later, delete the collections from inside it — the
photos and paperwork are cleaned up with them.

The demo carries no licence key and no trial stamp, so your fifteen days still
start on your own first launch.

## Updates

The app checks this page once at launch and offers anything newer in a dialog.
It is the only thing Collectionist ever sends over the network.

# Collectionist — releases

Installers for **Collectionist**, a local-first desktop collections manager.
This repository holds nothing else: no source, no issues, just the releases and
the `latest.json` every installed app reads on launch to find out whether a
newer version exists.

**[Download the latest release →](https://github.com/erwinohnehals/collectionist-releases/releases/latest)**

## What is in a release

| File                                | What it is                                                                                 |
| ----------------------------------- | ------------------------------------------------------------------------------------------ |
| `Collectionist_x.y.z_x64-setup.exe` | Windows installer. **This is the one to download.**                                        |
| `Collectionist_x.y.z_x64_en-US.msi` | The same app as an MSI, for deployment tooling.                                            |
| `*.sig`                             | Signatures the app checks before it installs an update. You never need to download these.  |
| `latest.json`                       | What the in-app updater reads.                                                             |

## Installing

Run the `.exe` and follow it. That is the whole procedure — there is nothing
else to download and nothing to unpack.

The installers are not code-signed yet, so Windows will say **"Windows
protected your PC"** on a first install: click **More info**, then **Run
anyway**. Updates applied from inside the app never show this again; they are
verified by the app's own signature instead.

## The first launch

The app asks one question and you answer it with a button:

- **Start with an example collection.** Vintage motorcycles and cars, with
  photographs, histories, invoices and saved filters, so there is something to
  look at before you have typed anything in. It comes with the app.
- **Start with an empty library**, and build your own from the beginning.

If you take the example and later want it gone, Settings empties it in one
press: the collections, their photographs and their paperwork all go, and the
item types stay, because those are what your own collections are built from.
As long as you have not started a collection of your own, Settings will also
put the example back.

The example carries no licence key and no trial stamp, so your trial starts on
your own first launch either way.

## Updates

The app checks this page once at launch and offers anything newer in a dialog.
It is the only thing Collectionist ever sends over the network.

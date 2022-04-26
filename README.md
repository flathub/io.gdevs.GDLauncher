# Issue Flowchart:

1. Is it on version 1.17+?

Yes: Continue to 2.

No: Continue to 3.

2. Have you tried using the latest version of java as outlined at the bottom of this readme?

Yes. The issue is still present: Continue to 3

No: Do that

3. Can you reproduce the issue using the upstream appimage version?

*Download the appimage from here: https://gdevs.io/#downloadContainer. Make it executable with `chmod +x xxx.appimage`. Run `./xxx.appimage`*

Yes, entirely: Consider reporting [upstream](https://github.com/gorilla-devs/GDLauncher/issues).

Yes, only partly: Report a good issue here with OS/hardware info, logs, crashdata, and anything else you consider important.

No: Report a good issue here with OS/hardware info, logs, crashdata, and anything else you consider important.

## How do I build this package?

The easiest way will be to have `flatpak-builder` installed and running:

```sh
flatpak-builder build-dir/ io.gdevs.GDLauncher.yml --force-clean --install --user
```

## How do I play versions of Minecraft that require Java non-LTS?

GDLauncher is sometimes behind in their java builds. To use the upstream flatpak Java:

Simply right click on the instance you wish to use flatpak Java for > Click "Manage" >
 Enable "Custom Java Path" > And map the path to `/app/jre/bin/java`
 
Then you should be good to go!

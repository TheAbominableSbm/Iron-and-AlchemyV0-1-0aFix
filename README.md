Initial release Alpha Version 0.1.0a has an issue with Forge Mod Loader not working upon clicking "play".


Instructions below detail how to resolve this issue. The next revision of will fix this.

1) Install the mod through Technic Launcher as normal.

2) Navigate to the install location which should look something like this:
"C:\Users\[YOURUSER]\AppData\Roaming\.technic\modpacks\[THISMODPACK]\bin

3) In this folder should be "modpack.jar". Rename this to simple "modpack" so that the ".jar" is no longer in the filename.

4) Click "Play". Minecraft should now launch with Forge Mod Loader with an alternate startup screen followed by confirmation of the mods
working (e.g. "38 mods loaded" on the title screen).

The issue with the file is that on my own system, the ".jar" was needed to compile the mod. However, upon downloading, this becomes
embedded in the name, therefore Java regards this as "modpack.jar.jar" meaning when it looks for "modpack.jar", it doesn't seem to exist.
"modpack..jar" is the file which contains the Forge self-loader and then becomes the Forge Mod Loader, hence why no mods load if this is
not named correctly.

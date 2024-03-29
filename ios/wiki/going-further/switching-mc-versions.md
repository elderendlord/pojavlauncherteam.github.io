# Pick a version. Any version.

In the official launcher, you can choose to use specific versions. PojavLauncher has this capability as well, although it's a bit trickier.

## Changing the versions
In the screen with the play button, tap the version number. A keyboard will present itself to you and you will now be able to change to the version you wish to use. Just make sure it's [supported](../../../about-pojavlauncher/supported-versions.md).

![](https://raw.githubusercontent.com/PojavLauncherTeam/website-assets/main/ios/MOV_0134.gif)

Versions like [Fabric](non-vanilla/fabric), [OptiFine](non-vanilla/optifine), and [Forge](non-vanilla/forge) require a bit of extra effort, read there pages to find out more about how to use them.

## Disclaimer

We need to talk.

Mods are pretty cool--extending the possible features of Minecraft with a simple file. The issue with mods on PojavLauncher for iOS is mainly just the memory limits make modding capabilities harder. If you install [PojavOptimize](performance), you may be able to circumvent this issue (as one of the mods included helps reduce memory usage). Small mods should run fine--especially if they only add blocks or it's OptiFine. Be careful with big mods, however, as either jetsam will kill the app or you'll run out of memory.

And now for shaders. Support for shaders is very limited, and you should expect to see some major issues if you're using a shader that hasn't been green-lighted. Sildur's Shaders works, and so does the Open4Es pack [here](https://github.com/Open4Es/Open4Es-Shader-Android) for **sure**, some others may work but they haven't been thoroughly documented as of this writing.

## Required step for v1.0 users

If you're still using version 1.0 for PojavLauncher, you'll need to make a file called `launcher_profiles.json` in /var/mobile/Documents/minecraft with the following contents:

```
{
  "profiles": {
    "(Default)": {
      "name": "(Default)",
      "lastVersionId": "Unknown"
    }
  },
  "selectedProfile": "(Default)"
}
```

Users with v1.1 or later do not need to do this--it's already done for you.

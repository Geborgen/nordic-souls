# Modification Guide

![Banner](https://raw.githubusercontent.com/Geborgen/nordic-souls/main/.github/NordicSoulsBanner.png)

<p align="center">
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/README.md">ReadMe</a> |
  <a href="https://www.nexusmods.com/skyrimspecialedition/mods/77497">Nexus</a> |
  <a href="https://discord.com/invite/9cRs3KPyuW">Discord</a> |
  <a href="https://ko-fi.com/geborgen">Ko-fi</a> |
  <a href="https://loadorderlibrary.com/lists/nordic-souls">Modlist</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md">Gameplay Guide</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/MODIFICATIONGUIDE.md">Modification Guide</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md">Changelog</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/FAQ.md">FAQ</a>
</p>

You are not guaranteed official support for modifying the list in any way, and you will void support for issues you encounter if you do. As mentioned in the [readme](https://github.com/Geborgen/nordic-souls/blob/main/README.md), Wabbajack's "rule 11" states that any modifications you make are done at your own risk. 

In the case of Nordic Souls, the list is often praised for how easily modifiable it is and how active the community around it is as well, so if you follow a few general guidelines and have a basic understanding of modding, you should have no trouble making the list your own.

It should be stated again that you do this at your own risk, and you are solely responsible for anything that breaks, whether or not you follow this guide. This guide will not provide incorrect information and will not intentionally try to break anything; however, is not exactly a step-by-step or hand-holding guide, as modding is a unique process for everyone. This is just a collection of things to pay attention to and otherwise basic instructions to follow as you make your modifications.

Check the community resources channel as well as the pins of the modifications channel in the [Discord](https://discord.com/invite/9cRs3KPyuW) for more in-depth guides written by the community. When modifying the list, you should use the modifications channel for support.

## Contents
- [Adding Mods](#adding-mods)
  - [Load Order](#load-order)
  - [Game Root](#game-root)
- [Modding Tools](#modding-tools)
  - [xEdit and Custom Patches](#xedit-and-custom-patches)
  - [BodySlide](#bodyslide)
  - [Synthesis](#synthesis)
  - [ParallaxGen](#parallaxgen)
  - [LOD Tools](#lod-tools)
- [List Updates](#list-updates)

## Adding Mods

This is not a modding guide. If you need a modding guide, there are many good resources on the internet. I put one together [here](https://sites.google.com/view/skyrimsemoddingguide). You should also check out [ModdingSkyrim](https://moddingskyrim.com/), [Lively's wiki](https://github.com/LivelyDismay/Learn-To-Mod/wiki), [Phoenix's guide](https://thephoenixflavour.com/bg/), and [biggie's videos](https://www.youtube.com/watch?v=5cHJ0i7hE2U&list=PLQVRNa_qhFsrNmcAn80ImEh0HXiTsNUyY). You can find more resources [here](https://sites.google.com/view/skyrimsemoddingguide/the-guide/other-resources). You should have some understanding of modding before you modify any list.

### Load Order

Nordic Souls has a carefully tuned load order, and as such, **you should *not* run LOOT** to sort mods. The full version of LOOT is not even installed. Do not use MO2's "sort" feature. *You should manually build around the existing load order.*

Know what mods you're adding. Read the mod pages, they should tell you where to place plugins, if it matters at all. Basic mods like armor sets generally don't matter. For the sake of this list, all plugins should be placed **above** `Water for ENB (Shades of Skyrim).esp`.

If you're comfortable with xEdit, you can use xEdit to check conflicts for mods you add. This can help determine proper load order.

The paper map plugins (`FWMF for Fantasy Paper Maps.esp` and all subsequent FWMF plugins) must be placed at the **very bottom** of the load order *at all times*, no exceptions. They must always be the last plugins to load, or else the map will be a blank purple (missing textures). If your map is missing or broken, double check that zero plugins load below the paper map.

If you think you messed up the load order, check the [Load Order Library link](https://loadorderlibrary.com/lists/nordic-souls) and expand `plugins.txt` to compare. It will always be on the latest version, so it might not be entirely accurate if you're modifying an earlier build.

### Game Root

Nordic Souls uses a "game root" setup, which includes a [stock game folder](https://github.com/The-Animonculory/Modding-Resources/blob/main/Stock%20Game%20Setup.md) as well as [Kezyma's Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720). If you add a mod that requires installation directly to the game folder like ReShade, you should instead install it to MO2 using the file structure outlined in the [Root Builder documentation](https://kezyma.github.io/?p=rootbuilder). To put it simply, install a mod with a folder called `Root` as the top directory, and then place the files that should be in the game folder in the root folder instead. If you need an example, you can view the list's installation of SKSE or ENB. *Ignore any warnings about an invalid mod installation.*

## Modding Tools

When modifying the list, you may have to regenerate various outputs. The general order for this is BodySlide > Synthesis > ParallaxGen > LOD.

The most commonly used tools are located in the toolbar located on the top right of MO2. To view additional tools included with the list, go to MO2's application drop-down below the toolbar.

Due to the stock game method, certain tools might not work by default. You can see how to change the game directory for most tools [here](https://github.com/The-Animonculory/Modding-Resources/blob/main/Stock%20Game%20Setup.md). If they aren't listed, you change them in either MO2's launch arguments, a settings menu within the tool, or you don't have to change anything at all.

If certain tools still aren't working correctly, you may have to change the game installation path in your computer's registry. You might need to do this if you install another list, as some change the registry path. Open the registry editor, and at the top bar type `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Bethesda Softworks\Skyrim Special Edition`. Double click `installed path` and change it to either Nordic Souls/Game Root the Steam installation path. [Here is an image if needed.](https://i.imgur.com/DfCAUYS.png) *This registry tweak is harmless, but should only be done if things aren't working correctly.* One of the tools that most commonly needs this fix is Synthesis.

### xEdit and Custom Patches

When adding mods, you should check them in xEdit for conflicts or errors. If you aren't comfortable with xEdit, it is a valuable tool to learn. You can use the [Tome of xEdit](https://tes5edit.github.io/docs/), [biggie's videos](https://www.youtube.com/watch?v=5cHJ0i7hE2U&list=PLQVRNa_qhFsrNmcAn80ImEh0HXiTsNUyY), and [GP's videos](https://www.youtube.com/watch?v=YCAmgBm6o8I&list=PLlN8weLk86XiGXJI4DaRa1QIq1zhDpD8V) as resources.

Nordic Souls has many custom patches, which you should only worry about if you're disabling mods. Most patches only have 2-3 mods as masters, so there should be no concern. If you want to create your own custom patches, check out [this video](https://www.youtube.com/watch?v=eO9B8xMWRP0) as well as [The Method](https://tes5edit.github.io/docs/6-themethod.html).

### BodySlide

BodySlide output should only be regenerated if you are adding custom outfits *that have BodySlide conversions* or changing body sliders within the program.

There will be no support provided for adding nudity to the list.

(section wip)

### Synthesis

If you add or disable mods, you might need to regenerate Synthesis output. The profile is included with the list, so all you really need to do is run it. Before running, you should temporarily disable the paper map plugins, ParallaxGen (PG) plugins, and DynDOLOD plugins.

To run Synthesis, simply run the program, check whichever group you wish to generate (circle filled; you can do all at once), and press the big arrow at the bottom. If you get compiling errors or are unable to run, you may have to relaunch the program. If you're still having trouble, reach out in the Discord modifications channel. There should be several plugins generated, but `Synthesis - IED Meshes.esp` is not needed and can be safely deleted.

### ParallaxGen

(section wip)

### LOD Tools

All requirements for LOD generation are installed. You should disable all paper map mods for the entire process (*the mods themselves*, not just the plugins; see the `Paper Map` separator), and re-enable them when all LOD tools are run.

Please refer to [Althro's written guide](https://github.com/The-Animonculory/Modding-Resources/blob/main/DynDOLOD.md) or [biggie's video guides](https://www.youtube.com/watch?v=5cHJ0i7hE2U&list=PLQVRNa_qhFsrNmcAn80ImEh0HXiTsNUyY) when generating LODs. You can skip steps involving grass LODs (although grass cache is provided if you're up for it) and ACMOS (NS uses a paper map).

## List Updates

When you update the list, you will loose all custom changes you make. Luckily, there is a workaround. For any mods that you add, prefix the mod name in MO2 with `[NoDelete]`, so the mod would be named `[NoDelete] NewMod`, for example. The mods will be thrown to the bottom of the priority list, but they will stay. To stop your added plugins from moving around, you can right-click them and select `Lock load order`. This might cause issues if the load order changes with an update, so double check the plugins list on Load Order Library.

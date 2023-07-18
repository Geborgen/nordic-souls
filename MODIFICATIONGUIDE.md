# Modification Guide

You are not guaranteed official support for modifying the list in any way, and you will void support for issues you encounter if you do. As mentioned in the [readme](https://github.com/Geborgen/nordic-souls/blob/main/README.md), Wabbajack's "rule 11" states that any modifications you make are done at your own risk. 

In the case of Nordic Souls, the list is often praised for how easily modifiable it is and how active the community around it is as well, so if you follow a few general guidelines and have a basic understanding of modding, you should have no trouble making the list your own.

It should be stated again that you do this at your own risk, and you are soley responsible for anything that breaks, whether or not you follow this guide. This guide will not provide incorrect information and will not intentionally try to break anything. This is not exactly a step-by-step guide, as modding is a unique process for everyone, rather it is a list of things to pay attention to, keep in mind, and otherwise basic instructions to follow as you make your modifications. With that out of the way, let's get started.

## Contents
- [Adding Mods](#adding-mods)
  - [Load Order](#load-order)
  - [Game Root](#game-root)
- [Managing Tools](#managing-tools)
  - [xEdit and Custom Patches](#xedit-and-custom-patches)
  - [Synthesis](#synthesis)
  - [EasyNPC](#easynpc)
  - [LOD Tools](#lod-tools)
- [List Updates](#list-updates)

## Adding Mods

This is not a modding guide. If you need a modding guide, there are many good resources on the internet. I put one together [here](https://sites.google.com/view/skyrimsemoddingguide). You should also check out [ModdingSkyrim](https://moddingskyrim.com/), [Lively's wiki](https://github.com/LivelyDismay/Learn-To-Mod/wiki), and [Phoenix's guide](https://thephoenixflavour.com/bg/). You can find more resources [here](https://sites.google.com/view/skyrimsemoddingguide/the-guide/other-resources). You should have some understanding of modding before you modify another list.

### Load Order

Nordic Souls has a carefully tuned load order, and as such, **you should not run LOOT** to sort mods, as my custom metadata doesn't carry over with Wabbajack. *You should build around the existing load order.*

Know what mods you're adding. Read the mod pages, they should tell you where to place plugins, if it matters at all. Basic mods like armor sets generally don't matter. For the sake of this list, all plugins should be placed **above** `Water for ENB (Shades of Skyrim).esp`. The paper map plugin, `NS_PaperMapMerge.esp`, must be placed at the **very bottom** of the load order *at all times*, no exceptions. It must always be the last plugin to load, or else the map will be a blank purple (missing textures). If your map is missing or broken, double check that zero plugins load below the paper map.

If you think you messed up the load order, check the [Load Order Library link](https://loadorderlibrary.com/lists/nordic-souls) and expand `plugins.txt` to compare. It will always be on the latest version, so it might not be entirely accurate if you're modifying an earlier build.

### Game Root

Nordic Souls uses a "game root" setup, which includes a [stock game folder](https://github.com/The-Animonculory/Modding-Resources/blob/main/Stock%20Game%20Setup.md) as well as [Kezyma's Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720). If you add a mod that requires installation directly to the game folder like ReShade, you should instead install it to MO2 using the file structure outlined in the [Root Builder documentation](https://kezyma.github.io/?p=rootbuilder). To put it simply, install a mod with a folder called `Root` as the top directory, and then place the files that should be in the game folder in the root folder instead. If you need an example, you can view the list's installation of SKSE or ENB. *Ignore any warnings about an invalid mod installation.*

## Managing Tools

To view additional tools included with the list, go to MO2's application drop-down and click `<Edit...>`, and disable `Hide in user interface` for any tool you need.

Due to the stock game method, certain tools might not work by default. You can see how to change the game directory for most tools [here](https://github.com/The-Animonculory/Modding-Resources/blob/main/Stock%20Game%20Setup.md). If they aren't listed, you change them in either MO2's launch arguments, a settings menu within the tool, or you don't have to change it at all.

If certain tools still aren't working correctly, you may have to change the game installation path in your computer's registry. You might need to do this if you install another list, as some change the registry path. Open the registry editor, and at the top bar type `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Bethesda Softworks\Skyrim Special Edition`. Double click `installed path` and change it to either Nordic Souls/Game Root the Steam installation path. [Here is an image if needed.](https://i.imgur.com/DfCAUYS.png) *This registry tweak is harmless, but should only be done if things aren't working correctly.* One of the tools that most commonly needs this fix is Synthesis.

### xEdit and Custom Patches

Nordic Souls has many custom patches, which you should only worry about if you're disabling mods. Most patches only have 2-3 mods as masters, so there should be no concern. If you want to create your own custom patches, check out [this video](https://www.youtube.com/watch?v=ErbiTZMRR6c) as well as [The Method](https://tes5edit.github.io/docs/6-themethod.html).

### Synthesis

IF you add or disable mods, you might need to regenerate Synthesis output. The profile is included with the list, so all you really need to do is run it. Before running, you should temporarily disable the paper map plugin.

### EasyNPC

Nordic Souls facegen is generated with EasyNPC. If you want to edit NPC appearances, [familiarize yourself with this tool](https://github.com/focustense/easymod/wiki/easynpc-%E2%80%90-Home). You will need to install the base NPC replacers which are not installed by default. They are downloaded though, and you can see the install order on Load Order Library by expanding `modlist.txt` and clicking `Show Disabled`, then finding the `NPC Appearances - EasyNPC` separator. Install accordingly, or install your own replacers. Disable all mods under that separator when the process is complete.

Make a backup of `NS_NPCFixes.esp` and disable it before the process, then restore it afterwards. This will fix broken khajiit (just disabling and re-enabling the plugin doesn't work). Alternatively, you can load all plugins related to Project ja-Kha'jay after the EasyNPC output plugins.

### LOD Tools

All requirements for LOD generation are installed. You should disable the paper map for the entire process, and disable Synthesis when running DynDOLOD.

Please refer to [Althro's DynDOLOD guide](https://github.com/The-Animonculory/Modding-Resources/blob/main/DynDOLOD.md) when generating LODs. You can skip steps involving Grass LODs (unless you want to generate grass cache and do it yourself; not easy to do on AE) and ACMOS (NS uses a paper map). [For reference, these are the settings that NS uses by default.](https://imgur.com/gallery/sTF2mBr) One thing not pictured are the default tree mesh rules, which are `LOD4/Billboard4, LOD8/Billboard4, LOD16/Billboard﻿(1)`.

## List Updates

When you update the list, you will loose all custom changes you make. Luckily, there is a workaround. For any mods that you add, prefix the mod name in MO2 with `[NoDelete]`, so the mod would be named `[NoDelete] NewMod`, for example. The mods will be thrown to the bottom of the priority list, but they will stay. To stop your added plugins from moving around, you can right-click them and select `Lock load order`. This might cause issues if the load order changes with the update, so double check the plugins list on Load Order Library.

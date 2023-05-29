# Nordic Souls

![NS2Screen](https://raw.githubusercontent.com/Geborgen/nordic-souls/main/.github/NS2Screen.png)

<p align="center">
  <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License</a>
</p>

<p align="center">
  <a href="https://geborgen.net/Nordic-Souls.html">Website</a> |
  <a href="https://www.nexusmods.com/skyrimspecialedition/mods/77497">Nexus Page</a> |
  <a href="https://discord.com/invite/9cRs3KPyuW">Discord Support</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md">Gameplay Guide</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/PERFORMANCEGUIDE.md">Performance Guide</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/KNOWNISSUES.md">Known Issues</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md">Changelog</a>
</p>

<p align="center">
  Please read this document in its entirety before playing the list.
</p>

## Contents
- [Preamble](#preamble)
- [List Contents](#list-contents)
- [System Requirements](#system-requirements)
  - [My Specs](#my-specs)
- [Installation](#installation)
  - [Anniversary Edition](#anniversary-edition)
  - [Preparations](#preparations)
    - [Pagefile](#pagefile)
  - [List Installation](#list-installation)
    - [Installing Wabbajack](#installing-wabbajack)
    - [Downloading and Installing the List](#downloading-and-installing-the-list)
    - [Problems with Installation](#problems-with-installation)
- [Post-Installation](#post-installation)
  - [Stock Game and Root Builder](#stock-game-and-root-builder)
  - [Customizing the List](#customizing-the-list)
    - [Performance](#performance)
    - [Optional Files](#optional-files)
    - [ENB](#enb)
    - [Widescreen Support](#widescreen-support)
    - [Gamepad Support](#gamepad-support)
- [Playing the List](#playing-the-list)
  - [Starting Up](#starting-up)
  - [Mod Configuration Menu](#mod-configuration-menu)
    - [Leveling Freedom](#leveling-freedom)
    - [SmoothCam](#smoothcam)
  - [Starting the Game](#starting-the-game)
  - [Gameplay Guide](#gameplay-guide)
- [Updating the List](#updating-the-list)
- [Uninstalling the List](#uninstalling-the-list)
- [Known Issues](#known-issues)
- [I found a bug!](#i-found-a-bug)
- [Changelog](#changelog)
- [Credits and Thanks](#credits-and-thanks)

## IMPORTANT: THIS LIST REQUIRES THE COMPLETE ANNIVERSARY EDITION UPGRADE. THIS MEANS THAT YOU MUST *PURCHASE* THE AE UPGRADE/DLC FROM STEAM.

## Preamble

Nordic Souls is a comprehensive gameplay and visual overhaul for Skyrim SE/AE which expands on the darker aspects of the game while still staying true to Skyrim's Nordic theme and modernizing it. Including dozens of hours of new quests, a complete SimonRim gameplay overhaul, beautiful yet performance-friendly visuals and much more, this list will modernize Skyrim in a way that is somewhat familiar yet new and refreshing.

Despite the name, this list does not attempt to "turn Skyrim into Dark Souls." There are of course influences from systems of Souls-like games, but ultimately the list is focused on modernizing Skyrim, not turning it into something else.

Nordic Souls is NOT a "vanilla+" list. The goal may have originally been to modernize Skyrim, but this includes changing almost every aspect of the game. It is still recognizably Skyrim, but different enough that it feels like a new game.

## List Contents

[The full list of mods can be viewed on Load Order Library.](https://loadorderlibrary.com/lists/nordic-souls)

[The default keymap can be found here.](http://www.keyboard-layout-editor.com/#/gists/75d0b99d7b2f35cd7f9433b87e83c93d)

## System Requirements

Nordic Souls requires ~273 GB of free space (including downloads). Without downloads, it's ~170 GB.

The list was built on a relatively low-tier machine, with older-gen parts. I run a 1080p 16:9 display.

### My Specs

- CPU: AMD Ryzen 5 2600
- GPU: NVIDIA GeForce GTX 1060 6GB
- RAM: 16GB DDR4

My specs are the minimum recommended for the best experience.

With the default ENB, in heavy areas (Falkreath/Riverwood) I might drop down to 35 FPS, but in most other exteriors I'll get closer to 55 FPS. Keep in mind my PC is by no means new, and this is without any of the performance tweaks. Many users report a stable high FPS in most or all areas of the game. If you need more performance, check out the [performance guide](https://github.com/Geborgen/nordic-souls/blob/main/PERFORMANCEGUIDE.md). With my PC being the minimum for a good experience, this list can be considered performance-friendly for most systems.

## Installation

I HIGHLY recommend you buy Nexus Premium before installing the list. You *technically* don't need it, but it will be an extremely long manual process if you don't have it. If you absolutely cannot buy premium, then put on a TV show or audiobook and make a day out it. 

If you are just updating the list, you can safely skip to [this section](#updating-the-list).

### Anniversary Edition
**Nordic Souls requires the full AE upgrade**, which means you must PURCHASE the Anniversary Edition upgrade/DLC. The list is built around every single CC item being installed, and will not function without them.

### Preparations

Please complete the following steps before the actual list installation:
1. Install [Visual C++ x64 Redistributables](https://aka.ms/vs/16/release/vc_redist.x64.exe).
2. Install [Microsoft .NET 5.0 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/5.0/runtime) AND [.NET 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
3. Set Skyrim to not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
4. Fully uninstall Skyrim by deleting the folders `/Steam/steamapps/common/Skyrim Special Edition and folder` and `/Documents/My Games/Skyrim Special Edition`, in addition to uninstalling through Steam.
5. Reinstall Skyrim into a location that is NOT in Program Files. Somewhere like `C:\Games` is a good location. [See this tutorial for moving Steam libraries.](https://www.youtube.com/watch?v=DSF1iWCqsM8)
6. Launch the game and download all Creation Club add-ons, this should happen automatically. When complete, close the game.

#### Pagefile

Large modlists require a lot of memory. If there isn't enough memory, it might fail to allocate more and cause a memory-related crash. You can fix this with a pagefile, which essentially acts as virtual memory.

To prevent memory crashes, perform the following steps to increase your pagefile size:
1. Press `Win + R` and enter `sysdm.cpl ,3`
2. Under the `Advanced` tab, press `Settings` under the `Performance` section
3. In the window that pops up, go to the `Advanced` tab and press `Change...` under the `Virtual Memory` section
4. Disable `Automatically manage paging file size for all drives`
5. If you have more than one drive, try enabling it for at least one more drive as a backup (make sure it has a decent bit of free space, like 15GB). Set the size to `System managed size`. Otherwise, set a custom size for the drive it's currently on and increase the maximum size to be at least 20GB.

### List Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://www.wabbajack.org/) and place it in a folder near or at the root of your drive, such as `C:\Wabbajack`. **Do not place it in Program Files, on your desktop, or in your downloads folder.**

#### Downloading and Installing the List

Downloading and installing Nordic Souls can take a long time depending on your internet connection and PC specs. I recommend you install it on an SSD, as everything will go much faster. Complete the steps below for installation:
1. Create a folder near the root of your drive called `Nordic Souls`.
2. Open Wabbajack, go to `Browse Modlists`, find Nordic Souls, and click the download arrow. Alternatively, download the .wabbajack file from this repository or the [Nexus page](https://www.nexusmods.com/skyrimspecialedition/mods/77497), add it to your Wabbajack folder, and open it.
3. Set your installation folder to the folder you made in step 1 (e.g. `C:\Nordic Souls`).
5. Your downloads folder should be set automatically. If it isn’t, set it to either `Nordic Souls\downloads` or another location. It can even be on another drive.
6. Click the start button to begin. Follow any prompts on-screen. *Reiterating from earlier: if you do not have Nexus Premium, you will have to manually click through each mod. There are over 1000 mods.*
7. Wait. It may take an hour or more depending on your connection. Read the rest of the readme and take a nap. If you have any errors during installation, see below. Otherwise, carry on to [post-installation](#post-installation) when completed.

#### Problems with Installation

Some common errors you may encounter during installation:
- Could not download x:
  - Large files can fail to download due to connection issues. You can either run Wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads (`Nordic Souls\downloads`).
  - Make sure you have purchased the Anniversary Edition upgrade, and launched the game through Steam to download all CC content.
- x is not a whitelisted download:
  - This may happen when I update the list. Please check if there is a new update or wait if there is none.
- Wabbajack could not find the game folder:
  - You will never get support for a pirated copy of the game. Either buy the game *on Steam* or, if you did, go back to the [Pre-Installation](#pre-installation) step.
- Antivirus reports a virus:
  - Windows 10/11 may automatically quarantine a key file that is needed for MO2. You can fix this by [adding an exclusion for MO2 in windows defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

If you are still having issues, visit the [Wabbajack Discord](https://discord.com/invite/wabbajack) or [my server](https://discord.com/invite/9cRs3KPyuW).

## Post-Installation

### Stock Game and Root Builder

Nordic Souls uses the [Stock Game](https://github.com/The-Animonculory/Modding-Resources/blob/main/Stock%20Game%20Setup.md) method. This is essentially a copy of Skyrim included with the installation folder. This means that everything is completely separate from your Steam installation of Skyrim (which is still required as the game files are not redistributed).

The list also uses [Kezyma's Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720) to keep the stock game folder clean. Any mod that needs to be installed to the game folder is instead added to MO2 with a special file structure, and is added to the game folder whenever the game is running.

### Customizing the List

**Other than what is mentioned here, modifying the list in any way will void all support.** I cannot guarantee that everything will work if you add or remove mods. If you do add mods that include plugins, they **MUST** load anywhere above the Synthesis patch, zero exceptions. The paper map plugin should always be at the very bottom of your load order.

As this may cause some confusion, I should clarify that I'm not against people editing the list. All I mean is that I won't be able to help if things break. This also falls under Wabbajack's rule 11, meaning that any modifications you make, you do so at your own risk.

Game settings and mod configs can be found in the `NS - Game Settings` mod under the `General Settings` separator in MO2. Right-click, open in explorer, and find the config you need, or click `Information...`, click the `INI Files` tab, and find what you need there. *If you're trying to configure a mod and it's not working, chances are it's being overwritten by a file from this mod.*

#### Performance

This list is designed to run well on most systems, but if you need more performance, check out the [performance guide](https://github.com/Geborgen/nordic-souls/blob/main/PERFORMANCEGUIDE.md).

#### Optional Files

Under the `Optional Files` separator, you can enable and disable things to your liking:
- [Performance Grass INI](https://www.nexusmods.com/skyrimspecialedition/mods/48689) makes the grass sparser for better performance. This file has the grass at about the minimum density before it begins to look awful. You can make it even sparser if you really want (higher number = less dense).
- [Nordic UI](https://www.nexusmods.com/skyrimspecialedition/mods/49881): Different UI style. Includes the full suit of Nordic UI-styled mods, for a consistent UI overhaul.
- [Skyrim Paper Map by Caro Tuts - LABELED VERSION](https://www.nexusmods.com/skyrimspecialedition/mods/62705): A labeled version of the paper map.

#### ENB

In-game, press `F10` to toggle the FPS counter, `F11` to open the ENB configuration menu, `F12` to toggle ENB, and `F7` to take a screenshot. These keybinds are the same for all included presets.

Nordic Souls uses a modified version of the incredible [Rudy ENB](https://www.nexusmods.com/skyrimspecialedition/mods/4796). By default, ambient occlusion is turned off, saving a lot of FPS. If you want better looking foliage or more depth and realism to shadows in general, turn on ambient occlusion in the ENB menu at the cost of 5-10 FPS.

If you want to change to one of the two other included presets, you must do the following:
1. Under the `ENB Presets` separator in MO2, **disable** `Mists of Tamriel for Rudy Obsidian`, `Rudy Obsidian Required Files`, and `Rudy ENB for Obsidian Weathers`.
2. Under the same separator, **enable** `Mists of Tamriel for Obsidian Weathers`, and either [Culminated ENB](https://www.nexusmods.com/skyrimspecialedition/mods/53167) or [Ominous ENB](https://www.nexusmods.com/skyrimspecialedition/mods/27333).
3. Make sure you only have one preset enabled at a time.
4. Launch your game as usual.

If you want to add a custom preset, you should familiarize yourself with [Kezyma's Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720), and match the way I've installed the presets to MO2.

If your interiors are too dark, edit `AmbientLightingIntensityInteriorDay` and `AmbientLightingIntensityInteriorNight` under the `Environment` category in the ENB menu.

If you do not want to use ENB, disable everything in that separator and keep it toggled off in-game.

#### Widescreen Support

- Enable `Widescreen Fix` under the `Widescreen Support` separator. This was made for 21:9 displays, but it should work fine for 32:9 displays.
- If you use the optional Nordic UI, enable `Nordic UI Widescreen Fix` in addition to the main widescreen fix.

#### Gamepad Support

For the purposes of this list, you can use the vanilla gamepad controlmap. The only thing you'll miss out on with the vanilla controlmap is dodging. You can change the dodge key in `TK Dodge RE.ini` to a gamepad key, but you may need to install a gamepad controlmap from the Nexus or make your own using [this tool](https://hawk.bar/SkyrimControlMapper/). You will not recieve official support for gamepad issues.

## Playing the List

### Starting Up

- Open the installation folder and open `ModOrganizer.exe`.
- Make sure the dropdown box on the right is set to `Play Nordic Souls [SKSE]` and run it.
- You can create a desktop shortcut in the shortcuts dropdown.
- **Do not launch the game through Steam.**

### Mod Configuration Menu

All MCMs have been pre-configured. Wait until all notifications on the top left are gone before opening the MCM. **Failure to do so can cause quite a few issues later on and will require you to start a new save.** You can tweak them to your liking if you want to customize your experience.

#### Leveling Freedom

By default, Nordic Souls uses the vanilla leveling system, but the nuances of it can be changed. In the Leveling Freedom MCM, you can adjust the leveling curve by selecting a preset or adjusting your own values. This will change how fast you level up in relation to your current level. See the [mod page](https://www.nexusmods.com/skyrimspecialedition/mods/69589) for more information.

#### SmoothCam

The Octavian preset is enabled by default. There are a few other options you can try. If you add your own, pay attention to the slot number.

### Starting the Game

Character creation has been overhauled. High Poly Head is selected automatically. Nordic Souls includes several character presets for you to choose from, but you can easily add your own.

You will spawn in a cell. **Wait until notifications have stopped appearing in the top right** and then locate the Statue of Mara to select your starting point. You can go through the vanilla intro sequence if you want, but I recommend exploring all the options.

### Gameplay Guide

The gameplay guide can be viewed [here](https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md). It includes a more in-depth explanation of what the list is actually trying to do, along with breaking down the different gameplay overhauls, quest mods, and other mods to pay attention to.

## Updating the List

Before updating, please check the [changelog](https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md) and back up your saves. You may need to start a new save after certain updates, this will be indicated in the changelog.

Updating is like installing the list. Make sure your paths are the same, and tick `overwrite existing modlist`. **Any changes you have made to the list will be reverted upon updating.** To keep mods that you added, prefix the mod name with `[NoDelete]`.

## Uninstalling the List

Simply delete the folder, and you have uninstalled the list.

## Known Issues

Please refer to [this page](https://github.com/Geborgen/nordic-souls/blob/main/KNOWNISSUES.md) before reporting an issue. Keep in mind that although I try to fix issues as they come up, I cannot fix everything. If your issue isn't listed, see below.

## I found a bug!

Visit the [issues](https://github.com/Geborgen/nordic-souls/issues) tab to see if your issue was already reported. If not, create a new issue. Please be as detailed as possible, and use the template provided.

## Changelog

To see the changes and version history, visit the [changelog](https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md).

## Credits and Thanks

- All mod authors for their hard work
- The Wabbajack team for making this awesome tool
- Other Wabbajack list authors for their help and inspiration
- The Community Helpers in my Discord server for their amazing assistance with ideas, testing, and community support
- Everyone who has played the list that has helped in some way, through finding issues and contributing ideas
- Waffles for the logo and branding
- Based Department (you know who you are)

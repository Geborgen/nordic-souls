# Nordic Souls

Modlist providing a visual and gameplay overhaul designed to "freshen up" and streamline Skyrim, while taking inspirations from other games yet still staying true to Skyrim's Nordic theme.

![NSLOGO](https://raw.githubusercontent.com/Geborgen/nordic-souls/main/.github/NSLOGO.webp)

<p align="center">
  <a href="https://www.nexusmods.com/skyrimspecialedition/mods/77497">Nexus Page</a> |
  <a href="https://discord.com/invite/nsJquPrHHE">Discord Support</a> |
  <a href="https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md">Gameplay Guide</a> |
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
- [Installation](#installation)
  - [Anniversary Edition](#anniversary-edition)
  - [Preparations](#preparations)
    - [Pagefile](#pagefile)
  - [List Installation](#list-installation)
    - [Installing Wabbajack](#installing-wabbajack)
    - [Downloading and Installing the List](#downloading-and-installing-the-list)
    - [Problems with Installation](#problems-with-installation)
- [Post-Installation](#post-installation)
  - [Stock Game](#stock-game)
  - [ENB](#enb)
  - [Customizing the List](#customizing-the-list)
- [Playing the List](#playing-the-list)
  - [Starting Up](#starting-up)
  - [Mod Configuration Menu](#mod-configuration-menu)
  - [Starting the Game](#starting-the-game)
  - [Gameplay Guide](#gameplay-guide)
- [Updating the List](#updating-the-list)
- [Uninstalling the List](#uninstalling-the-list)
- [Known Issues](#known-issues)
- [I found a bug!](#i-found-a-bug)
- [Changelog](#changelog)
- [Credits and Thanks](#credits-and-thanks)

## THIS LIST REQUIRES THE COMPLETE AE UPGRADE.

## Preamble

Nordic Souls is a comprehensive gameplay and visual overhaul for Skyrim SE/AE which expands on the darker aspects of the game while still staying true to Skyrim's Nordic theme and modernizing it. Including LOTD, dozens of hours of new quests, a complete SimonRim gameplay overhaul, and much more, this list will modernize Skyrim in a way that is somewhat familiar yet new and refreshing.

Despite the name, this list does not attempt to "turn Skyrim into Dark Souls." There are of course influences from systems of Souls-like games, but ultimately the list is focused on modernizing Skyrim, not turning it into something else.

Nordic Souls is NOT a "vanilla+" list. The goal may have originally been to modernize Skyrim, but this includes changing almost every aspect of the game. It is still recognizably Skyrim, but different enough that it feels like a new game.

## List Contents
[The full list of mods can be viewed on Load Order Library.](https://loadorderlibrary.com/lists/nordic-souls)

## System Requirements

Nordic Souls was built on a low-to-mid-tier machine, with slightly older-gen parts. I run a 1080p 16:9 display.

### My Specs
- CPU: AMD Ryzen 5 2600
- GPU: NVIDIA GeForce GTX 1060 6GB
- RAM: 16GB DDR4

My specs are the minimum recommended for the best experience. I get around 40-50 FPS in most exteriors.

The list requires ~220GB of free space (including downloads). Without downloads, it's ~142GB.

## Installation

I HIGHLY recommend you buy Nexus Premium before installing the list. You *technically* don't need it, but it will be an extremely long manual process if you don't have it. If you are just updating the list, you can safely skip to [this section](#updating-the-list).

### Anniversary Edition
**Nordic Souls requires the full AE upgrade**, which means you must PURCHASE the Anniversary Edition add-on DLC. The list is built around every single CC item being installed, and will not function without them.

### Preparations

Please complete the following steps before the actual list installation.

1. Install [Visual C++ x64 Redistributables](https://aka.ms/vs/16/release/vc_redist.x64.exe).
2. Install [Microsoft .NET 5.0 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/5.0/runtime) AND [.NET 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
3. Set Skyrim to not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
4. Fully uninstall Skyrim by deleting the folders `/Steam/steamapps/common/Skyrim Special Edition and folder` and `/Documents/My Games/Skyrim Special Edition`.
5. Reinstall Skyrim into a location that is NOT in Program Files. Somewhere like `C:\Games` is a good location. [See this tutorial for moving Steam libraries.](https://www.youtube.com/watch?v=DSF1iWCqsM8)
6. Launch the game and download all Creation Club add-ons, this should happen automatically. When complete, close the game.

#### Pagefile

Large modlists require a lot of memory. If there isn't enough memory, it might fail to allocate more and cause a memory-related crash. You can fix this with a pagefile, which essentially acts as virtual memory. A

To prevent memory crashes, perform the following steps to increase your pagefile size.

1. Press `Win + R` and enter `sysdm.cpl ,3`
2. Under the `Advanced` tab, press `Settings` under the `Performance` section
3. In the window that pops up, go to the `Advanced` tab and press `Change...` under the `Virtual Memory` section
4. Disable `Automatically manage paging file size for all drives`
5. If you have more than one drive, try enabling it for at least one more drive as a backup (make sure it has a decent bit of free space, like 15GB). Set the size to `System managed size`. Otherwise, set a custom size for the drive it's currently on and increase the maximum size to be at least 20GB.

### List Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases) and place it in a folder near or at the root of your drive, such as `C:\Wabbajack`. **Do not place it in Program Files, on your desktop, or in your downloads folder.**

#### Downloading and Installing the List

Downloading and installing Nordic Souls can take a long time depending on your internet connection and PC specs. I recommend you install it on an SSD, as everything will go much faster. Complete the steps below for installation.

1. Create a folder near the root of your drive called `Nordic Souls`.
2. Download the .wabbajack file and open it.
3. Set your installation folder to the folder you made in step 1 (e.g. `C:\Nordic Souls`).
5. Your downloads folder should be set automatically. If it isn’t, set it to `Nordic Souls\downloads`.
6. Click the start button to begin. Follow any prompts on-screen. *Reiterating from earlier: if you do not have Nexus Premium, you will have to manually click through each mod. There are over 700 mods.*
7. Wait. It may take an hour or more depending on your connection. Read the rest of the readme and take a nap. If you have any errors during installation, see below. Otherwise, carry on to [post-installation](#post-installation) when completed.

#### Problems with Installation

Some common errors you may encounter during installation are listed below.

- Could not download x:
  - Big files can fail to download due to connection issues. You can either run Wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads (`Nordic Souls\downloads`).
- x is not a whitelisted download:
  - This may happen when I update the list. Please check if there is a new update or wait if there is none.
- Wabbajack could not find my game folder:
  - You will never get support for a pirated copy of the game. Either buy the game *on Steam* or, if you did, go back to the [Pre-Installation](#pre-installation) step.
- Antivirus reports a virus:
  - Windows 10/11 may automatically quarantine a key file that is needed for MO2. You can fix this by [adding an exclusion for MO2 in windows defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

If you are still having issues, visit the [Wabbajack Discord](https://discord.com/invite/wabbajack). *Do not use my server for Wabbajack support.*

## Post-Installation

### Stock Game

Nordic Souls includes the **Stock Game** feature. This is essentially a copy of Skyrim included with the installation folder, which has cleaned plugins and all required files. This means that everything is completely separate from your Steam installation of Skyrim (which is still required as the game files are not redistributed). Basically, you don't need to transfer any files to your game folder.

### ENB

Nordic Souls includes a slightly modified version of the incredible [Rudy ENB](https://www.nexusmods.com/skyrimspecialedition/mods/4796). Press `F10` to toggle the FPS counter, `F11` to open the ENB configuration menu, and `F12` to toggle the ENB.

If you want to change the ENB, you must do the following:

- Ensure the ENB you want works with [Obsidian Weathers](https://www.nexusmods.com/skyrimspecialedition/mods/12125/) and [Lux](https://www.nexusmods.com/skyrimspecialedition/mods/43158).
- Disable the `Rudy ENB Required Files` mod, located in the `LIGHTING` separator in MO2.
- Delete all files in `Nordic Souls\Stock Game` that start with `enb`.
- Install the preset into the Stock Game folder.

If you want to fully remove ENB, delete `d3d11.dll` and `d3dcompiler_46e.dll`.

### Customizing the List

Under the `OPTIONAL CONTENT` separator, you can enable and disable things to your liking. This includes a widescreen fix: If you use a widescreen monitor, enable this, and check the [Untarnished UI](https://www.nexusmods.com/skyrimspecialedition/mods/75188) mod page for additional instructions.

You can also enable mods such as [NVIDIA Reflex Support](https://www.nexusmods.com/skyrimspecialedition/mods/74498) for more performance if you have an NVIDIA GPU and [Camera Noise](https://www.nexusmods.com/skyrimspecialedition/mods/77185) for a more lively camera. [Apothecary - Vanilla Potion Restore](https://www.nexusmods.com/skyrimspecialedition/mods/78230) is also under this category if you don't like it.

**Other than this, modifying the list in any way will void all support.** I cannot guarantee that everything will work if you add or remove mods.

## Playing the List

### Starting Up

Open the installation folder and open `ModOrganizer.exe`.

Make sure the dropdown box on the right is set to `Play Nordic Souls [SKSE]` and run it.

You can create a desktop shortcut in the shortcuts dropdown.

**Do not launch the game through Steam.**

### Mod Configuration Menu

All MCMs have been pre-configured. Wait until all notifications on the top left are gone before opening the MCM. **Failure to do so will cause quite a few issues later on and will require you to start a new save.** You can tweak them to your liking if you want to customize your experience.

### Starting the Game

Character creation has been overhauled. High Poly Head should be selected automatically. Nordic Souls does not include any character presets, but you can easily add presets yourself by installing them like normal mods (ensure they use HPH). *If your character is frozen at first, just change the race. This is a known issue with Precision.*

You will spawn in a cell. **Wait until notifications have stopped appearing in the top right** and then locate the Statue of Mara to select your starting point. You can go through the vanilla intro sequence if you want, but I recommend exploring all the options.

### Gameplay Guide

The gameplay guide can be viewed [here](https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md). It includes a more in-depth explanation of what the list is actually trying to do, along with breaking down the different gameplay overhauls, quest mods, and other mods to pay attention to.

## Updating the List

Before updating, please check the [changelog](https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md) and back up your saves. You may need to start a new save after certain updates, this will be indicated in the changelog.

Updating is like installing the list. Make sure your paths are the same, and tick `overwrite existing modlist`. **Any changes you have made to the list will be reverted upon updating.**

## Uninstalling the List

Just delete the folder. The Stock Game feature makes this simple.

## Known Issues

Please refer to [this page](https://github.com/Geborgen/nordic-souls/blob/main/KNOWNISSUES.md) before reporting an issue. Keep in mind that although I try to fix issues as they come up, I cannot fix everything. If your issue isn't listed, see below.

## I found a bug!

Visit the [issues](https://github.com/Geborgen/nordic-souls/issues) tab to see if your issue was already reported. If not, create a new issue. Please be as detailed as possible, and use the template provided.

## Changelog

To see the changes and version history, visit the [changelog](https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md).

## Credits and Thanks

- All mod authors for their hard work
- The Wabbajack team for making this awesome tool
- Monitor144 and Olivinism for playtesting
- Styyx for helping troubleshoot a lot of Wabbajack errors
- Based Department (you know who you are)

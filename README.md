# Nordic Souls

![NSLOGO](https://raw.githubusercontent.com/Geborgen/nordic-souls/main/.github/NSLOGO.webp)

<p align="center">
  <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License</a>
</p>

<p align="center">
  <a href="https://geborgen.net/Nordic-Souls.html">Website</a> |
  <a href="https://www.nexusmods.com/skyrimspecialedition/mods/77497">Nexus Page</a> |
  <a href="https://discord.com/invite/9cRs3KPyuW">Discord Support</a> |
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
  - [Stock Game](#stock-game)
  - [Customizing the List](#customizing-the-list)
    - [ENB](#enb)
    - [Optional Content](#optional-content)
    - [Widescreen Support](#widescreen-support)
    - [Gamepad Support](#gamepad-support)
- [Playing the List](#playing-the-list)
  - [Starting Up](#starting-up)
  - [Mod Configuration Menu](#mod-configuration-menu)
    - [Easy WheelMenu](#easy-wheelmenu) 
    - [The Ultimate Dodge Mod](#the-ultimate-dodge-mod)
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

Nordic Souls is a comprehensive gameplay and visual overhaul for Skyrim SE/AE which expands on the darker aspects of the game while still staying true to Skyrim's Nordic theme and modernizing it. Including LOTD, dozens of hours of new quests, a complete SimonRim gameplay overhaul, and much more, this list will modernize Skyrim in a way that is somewhat familiar yet new and refreshing.

Despite the name, this list does not attempt to "turn Skyrim into Dark Souls." There are of course influences from systems of Souls-like games, but ultimately the list is focused on modernizing Skyrim, not turning it into something else.

Nordic Souls is NOT a "vanilla+" list. The goal may have originally been to modernize Skyrim, but this includes changing almost every aspect of the game. It is still recognizably Skyrim, but different enough that it feels like a new game.

## List Contents
[The full list of mods can be viewed on Load Order Library.](https://loadorderlibrary.com/lists/nordic-souls)

[The default keymap can be found here.](http://www.keyboard-layout-editor.com/#/gists/75d0b99d7b2f35cd7f9433b87e83c93d)

## System Requirements

Nordic Souls requires ~273 GB of free space (including downloads). Without downloads, it's ~170 GB.

The list was built on a low-to-mid-tier machine, with slightly older-gen parts. I run a 1080p 16:9 display.

### My Specs
- CPU: AMD Ryzen 5 2600
- GPU: NVIDIA GeForce GTX 1060 6GB
- RAM: 16GB DDR4

My specs are the minimum recommended for the best experience. 

With the default ENB, in heavy areas (Falkreath/Riverwood) I might get ~35 FPS, but in most other exteriors I'll get closer to 50 FPS. In interiors, I'll keep a steady 60. Many users report a stable high FPS in most or all areas of the game.

## Installation

I HIGHLY recommend you buy Nexus Premium before installing the list. You *technically* don't need it, but it will be an extremely long manual process if you don't have it. If you absolutely cannot buy premium, then put on a TV show or audiobook and make a day out it. 

If you are just updating the list, you can safely skip to [this section](#updating-the-list).

### Anniversary Edition
**Nordic Souls requires the full AE upgrade**, which means you must PURCHASE the Anniversary Edition upgrade/DLC. The list is built around every single CC item being installed, and will not function without them.

### Preparations

Please complete the following steps before the actual list installation.

1. Install [Visual C++ x64 Redistributables](https://aka.ms/vs/16/release/vc_redist.x64.exe).
2. Install [Microsoft .NET 5.0 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/5.0/runtime) AND [.NET 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
3. Set Skyrim to not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
4. Fully uninstall Skyrim by deleting the folders `/Steam/steamapps/common/Skyrim Special Edition and folder` and `/Documents/My Games/Skyrim Special Edition`, in addition to uninstalling through Steam.
5. Reinstall Skyrim into a location that is NOT in Program Files. Somewhere like `C:\Games` is a good location. [See this tutorial for moving Steam libraries.](https://www.youtube.com/watch?v=DSF1iWCqsM8)
6. Launch the game and download all Creation Club add-ons, this should happen automatically. When complete, close the game.

#### Pagefile

Large modlists require a lot of memory. If there isn't enough memory, it might fail to allocate more and cause a memory-related crash. You can fix this with a pagefile, which essentially acts as virtual memory.

To prevent memory crashes, perform the following steps to increase your pagefile size.

1. Press `Win + R` and enter `sysdm.cpl ,3`
2. Under the `Advanced` tab, press `Settings` under the `Performance` section
3. In the window that pops up, go to the `Advanced` tab and press `Change...` under the `Virtual Memory` section
4. Disable `Automatically manage paging file size for all drives`
5. If you have more than one drive, try enabling it for at least one more drive as a backup (make sure it has a decent bit of free space, like 15GB). Set the size to `System managed size`. Otherwise, set a custom size for the drive it's currently on and increase the maximum size to be at least 20GB.

### List Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://www.wabbajack.org/) and place it in a folder near or at the root of your drive, such as `C:\Wabbajack`. **Do not place it in Program Files, on your desktop, or in your downloads folder.**

#### Downloading and Installing the List

Downloading and installing Nordic Souls can take a long time depending on your internet connection and PC specs. I recommend you install it on an SSD, as everything will go much faster. Complete the steps below for installation.

1. Create a folder near the root of your drive called `Nordic Souls`.
2. Open Wabbajack, go to `Browse Modlists`, find Nordic Souls, and click the download arrow. Alternatively, download the .wabbajack file from this repository or the [Nexus page](https://www.nexusmods.com/skyrimspecialedition/mods/77497), add it to your Wabbajack folder, and open it.
3. Set your installation folder to the folder you made in step 1 (e.g. `C:\Nordic Souls`).
5. Your downloads folder should be set automatically. If it isn’t, set it to either `Nordic Souls\downloads` or another location. It can even be on another drive.
6. Click the start button to begin. Follow any prompts on-screen. *Reiterating from earlier: if you do not have Nexus Premium, you will have to manually click through each mod. There are over 1000 mods.*
7. Wait. It may take an hour or more depending on your connection. Read the rest of the readme and take a nap. If you have any errors during installation, see below. Otherwise, carry on to [post-installation](#post-installation) when completed.

#### Problems with Installation

Some common errors you may encounter during installation are listed below.

- Could not download x:
  - Big files can fail to download due to connection issues. You can either run Wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads (`Nordic Souls\downloads`).
  - Make sure you have purchased the Anniversary Edition upgrade, and launched the game through Steam to download all CC content.
- x is not a whitelisted download:
  - This may happen when I update the list. Please check if there is a new update or wait if there is none.
- Wabbajack could not find the game folder:
  - You will never get support for a pirated copy of the game. Either buy the game *on Steam* or, if you did, go back to the [Pre-Installation](#pre-installation) step.
- Antivirus reports a virus:
  - Windows 10/11 may automatically quarantine a key file that is needed for MO2. You can fix this by [adding an exclusion for MO2 in windows defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

If you are still having issues, visit the [Wabbajack Discord](https://discord.com/invite/wabbajack) or [my server](https://discord.com/invite/9cRs3KPyuW).

## Post-Installation

### Stock Game

Nordic Souls includes the **Stock Game** feature. This is essentially a copy of Skyrim included with the installation folder, which has cleaned plugins and all required files. This means that everything is completely separate from your Steam installation of Skyrim (which is still required as the game files are not redistributed). Basically, you don't need to transfer any files to your game folder.

### Customizing the List

**Other than what is mentioned here, modifying the list in any way will void all support.** I cannot guarantee that everything will work if you add or remove mods. If you do add mods that include plugins, they **MUST** load anywhere above the Synthesis patch, zero exceptions. The paper map plugin should always be at the very bottom of your load order.

As this may cause some confusion, I should clarify that I'm not against people editing the list. All I mean is that I won't be able to help if things break. This also falls under Wabbajack's rule 11, meaning that any modifications you make, you do so at your own risk.

Game settings and mod configs can be found in the `[NoDelete] NS - Game Settings` mod under the `WRAPPING UP - OUTPUT` separator in MO2. Right-click, open in explorer, and find the config you need. If you're trying to configure a mod and it's not working, chances are it's being overwritten by a file from this mod.

#### ENB

Nordic Souls uses a slightly modified version of the incredible [Rudy ENB](https://www.nexusmods.com/skyrimspecialedition/mods/4796) by default,, however there are a few alternative presets to choose from. Press `F10` to toggle the FPS counter, `F11` to open the ENB configuration menu, `F12` to toggle the ENB, and `F7` to take a screenshot. These keybinds are the same for all included ENBs.

If you want to change the ENB, you must do the following.

1. Under the `WRAPPING UP - ENB` separator in MO2, **disable** `Mists of Tamriel for Rudy Obsidian` and `Rudy ENB Required Files`.
2. Under the same separator, **enable** `Mists of Tamriel for Obsidian Weathers` and `ENB Night Eye Fix`.
3. In the dropdown in the top right of MO2, change the program to `ENB Organizer`.
4. Run it and ignore any warning about Nexus updates.
5. Click the three bars on the top left and navigate to the `Presets` tab.
6. Disable Rudy ENB with the toggle on the bottom of the card, and enable any other ENB (see [here](https://imgur.com/gallery/3WDkZit) for a higher quality comparison).
7. Make sure you only have one ENB enabled at a time.
8. Launch your game as usual.

Adding new ENBs or changing weather mods is possible but not supported.

If you do not want to use ENB, keep it toggled off.

#### Optional Content

Under the `WRAPPING UP - OPTIONAL CONTENT` separator, you can enable and disable things to your liking:
- [Apothecary - Vanilla Potion Restore](https://www.nexusmods.com/skyrimspecialedition/mods/78230) is **enabled** by default. Disable if you prefer Apothecary's restore-over-time system. If you re-enable, the ESP placement doesn't matter as long as it loads after Apothecary and before the Synthesis patch.
- [Alternate Conversation Camera Plus](https://www.nexusmods.com/skyrimspecialedition/mods/40722) is **enabled** by default. Disable if you don't want zoom effect during dialogue.
- [Camera Noise](https://www.nexusmods.com/skyrimspecialedition/mods/77185) is **enabled** by default. Disable if you don't like the subtle camera-shake effect.
- [Rumble](https://www.nexusmods.com/skyrimspecialedition/mods/84507) is **enabled** by default. Disable if you don't like the improved controller rumble.
- [NORDIC UI Full Suite](https://www.nexusmods.com/skyrimspecialedition/mods/49881) is **disabled** by default. Enable if you want a different UI style.
- [Enhanced Blood Textures - No Screen Blood](https://www.nexusmods.com/skyrimspecialedition/mods/2357) is **disabled** by default. Enable if you don't like the screen blood that EBT adds.
- [Kaidan 2 Fart Patch](https://kaidanmod.com/) is **disabled** by default. Enable to make Kaidan fart. Only if you're close, though.

#### Widescreen Support

- Enable `Widescreen Fix` under the `WRAPPING UP - OPTIONAL CONTENT` separator. This was made for 21:9 displays, but it *should* work fine for 32:9 displays.
- If you use the optional Nordic UI, enable the previous mod, and `NORDIC UI Widescreen Fix` (below the previous mod).
- Recommended settings you should change yourself:
  - SkyHUD - fMessageInfoPosX = `1030`
  - TrueHUD - Player Widget Anchor X = `-0.105` 
  - TrueHUD - Player Loot Anchor X = `1.17`

#### Gamepad Support

Vanilla gamepad support is... fine. For the purposes of this list, you can use the vanilla gamepad controlmap. See [this section](#the-ultimate-dodge-mod) for a recommended tweak to make dodging work correctly.

## Playing the List

### Starting Up

- Open the installation folder and open `ModOrganizer.exe`.
- Make sure the dropdown box on the right is set to `Play Nordic Souls [SKSE]` and run it.
- You can create a desktop shortcut in the shortcuts dropdown.
- **Do not launch the game through Steam.**

### Mod Configuration Menu

All MCMs have been pre-configured. Wait until all notifications on the top left are gone before opening the MCM. **Failure to do so will cause quite a few issues later on and will require you to start a new save.** You can tweak them to your liking if you want to customize your experience.

#### Easy WheelMenu

Easy WheelMenu requires special configuration.

- Open the `EasyWheel` MCM, go to `Maintenance`, and press `Load` under `User Settings`. 
- Go to `General`, un-tick `Hide Spells`, then tick it again.

Easy WheelMenu is now configured. Press `K` to use it.

#### The Ultimate Dodge Mod

If you use gamepad, you may want to configure TUDM.

- Open the `The Ultimate Dodge Mod` MCM, go to `General`, and tick `Gamepad/Controller Compatibility`.
- Pick your sneak style:
  - Sneak Style 1 (recommended): Dodge with left thumb while weapon is drawn and/or in combat, sneak otherwise.
  - Sneak Style 2: Dodge with left thumb while weapon is drawn, sneak otherwise.
  
TUDM is now configured for gamepad usage.

#### Leveling Freedom

By default, Nordic Souls uses the vanilla leveling system, but the nuances of it can be changed. In the Leveling Freedom MCM, you can adjust the leveling curve by selecting a preset or adjusting your own values. This will change how fast you level up in relation to your current level. See the [mod page](https://www.nexusmods.com/skyrimspecialedition/mods/69589) for more information.

#### SmoothCam

The Octavian preset is enabled by default. There are a few other options you can try. If you add your own, pay attention to the slot number.

### Starting the Game

Character creation has been overhauled. High Poly Head is selected automatically. Nordic Souls does not include any character presets, but you can easily add presets yourself by installing them like normal mods (their placement in the mod list doesn't matter). Ensure that installed presets use HPH.

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
- Styyx for helping troubleshoot a lot of Wabbajack errors
- All the members of my Discord who have helped develop the list, through finding issues and contributing ideas
- Based Department (you know who you are)

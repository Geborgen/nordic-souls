# Nordic Souls

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

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

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
    - [Prerequisites](#prerequisites)
    - [Pagefile and Crash Prevention](#pagefile-and-crash-prevention)
    - [Shader Cache Size](#shader-cache-size)
    - [Steam Setup](#steam-setup)
    - [Installing CC Content](#installing-cc-content)
  - [List Installation](#list-installation)
    - [Installing Wabbajack](#installing-wabbajack)
    - [Downloading and Installing the List](#downloading-and-installing-the-list)
    - [Problems with Installation](#problems-with-installation)
- [Post-Installation](#post-installation)
  - [Stock Game and Root Builder](#stock-game-and-root-builder)
  - [Antivirus Exeptions](#antivirus-exceptions)
  - [Customizing the List](#customizing-the-list)
    - [Optional Files](#optional-files)
    - [ENB](#enb)
    - [Community Shaders](#community-shaders)
    - [Widescreen Support](#widescreen-support)
    - [Gamepad Support](#gamepad-support)
    - [Performance Tweaks](#performance-tweaks)
    - [Modification Guide](#modification-guide)
- [Playing the List](#playing-the-list)
  - [Starting Up](#starting-up)
    - [Controls](#controls)
  - [Mod Configuration Menu](#mod-configuration-menu)
  - [Starting the Game](#starting-the-game)
  - [Gameplay Guide](#gameplay-guide)
  - [Note for Content Creators](#note-for-content-creators)
- [Updating the List](#updating-the-list)
- [Uninstalling the List](#uninstalling-the-list)
- [Known Issues](#known-issues)
- [I found a bug!](#i-found-a-bug)
- [Changelog](#changelog)
- [FAQ](#faq)
- [Credits and Thanks](#credits-and-thanks)

> [!IMPORTANT]
> This list **requires** the complete Anniversary Edition upgrade. This means that you must *purchase* the AE upgrade/DLC from Steam.

## Preamble

Nordic Souls is a comprehensive visual and gameplay overhaul designed to modernize Skyrim while staying true to the game's Nordic theme. It provides a perfect balance between plenty of new content, a complete SimonRim gameplay overhaul, and beautiful yet performance-friendly visuals.

Despite the name, this list does not attempt to "turn Skyrim into Dark Souls." This list is focused on modernizing Skyrim, not turning the game into something else.

Everything about the game is improved, but still recognizably Skyrim. Tons of new quests have been added and loads of new gear is naturally integrated on top of a beautiful (and customizable!) graphics overhaul. You'll also find a lightweight gameplay overhaul that improves mechanics while adding cool new features. No matter what, you'll always find something to do. Have fun!

## List Contents

The full list of mods can be found on [Load Order Library](https://loadorderlibrary.com/lists/nordic-souls).

A more in-depth look at the mods used can be found in the [gameplay guide](https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md).

## System Requirements

| Minimum | Recommended |
|-----|-----|
| Intel i5-9400 / AMD Ryzen 5 2600x | Intel i5-13400 / AMD Ryzen 5 5600x  |
| NVIDIA GTX 1060 / AMD RX 580 | NVIDIA RTX 3060 TI / AMD RX 6700 |
| 16 GB DDR4 | 32 GB DDR4 |
| SATA SSD | NVMe SSD |

Many users report high FPS in most areas. This list is performance-friendly on almost any machine. The specs listed above are for 60 FPS, you can go lower if you don't mind losing some frames. Refer to the [performance section](#performance-tweaks) for more information.

The Nordic Souls installation requires a total of ~271 GB. This is broken down into a ~97 GB download size and a ~174 GB installation size. Keep in mind that Wabbajack requires around 30 GB of extra space on your main drive for temporary and working files during installation, which is roughly accounted for in the UI.

> [!TIP]
> If the space requirement is uncomfortable, remember that you can delete downloads once the list is successfully installed. You can also set your download location to a different drive than the installation location; more on that later.

## Installation

If you are just updating the list, you can safely skip to [this section](#updating-the-list).

> [!TIP]  
> I HIGHLY recommend you buy Nexus Premium before installing the list. You *technically* don't need it, but it will be an extremely long manual process if you don't have it. If you absolutely cannot buy premium, then put on a TV show or audiobook and make a day out it. 

### Anniversary Edition

**Nordic Souls requires the full AE upgrade**, which means you must PURCHASE the Anniversary Edition upgrade/DLC. The list is built around every single CC item being installed, and will not function without them.

### Preparations

#### Prerequisites

Please complete the following steps:
1. Install [Visual C++ x64 Redistributables](https://aka.ms/vs/17/release/vc_redist.x64.exe).
2. Install [Microsoft .NET 9.0 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/9.0) (both `console apps` and `desktop apps` x64).
3. Fully disable OneDrive and any other programs that hook into user file areas.
4. Reinstall Skyrim into a location that is not Program Files. Somewhere like `C:\Games` is a good location. If you only have one drive, look into [LostDragonist's SteamLibrary tool](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide). You should have the latest version of Skyrim, version `1.6.1170`. **Do not verify file integrity, as this will cause issues.**
5. Set Skyrim to not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
6. Right click Skyrim in Steam, click `Properties`, disable `Enable the Steam overlay while in-game`.

#### Pagefile and Crash Prevention

Large modlists require a lot of memory. If there isn't enough memory, it might fail to allocate more and cause a memory-related crash. You can fix this with a pagefile, which essentially acts as virtual memory.

To prevent memory crashes, perform the following steps to increase your pagefile size:
1. Press `Win + R` and enter `sysdm.cpl ,3`
2. Under the `Advanced` tab, press `Settings` under the `Performance` section
3. In the window that pops up, go to the `Advanced` tab and press `Change...` under the `Virtual Memory` section
4. Disable `Automatically manage paging file size for all drives`
5. Select your disk drive, ideally your fasted SSD
6. Under the `Custom Size:` option, change `Initial Size (MB)` and `Maximum Size (MB)` to `20480`
7. Click `Set`
8. Click `OK`, then `Apply` and `OK`
9. Restart your computer

#### Shader Cache Size

If you have an NVIDIA graphics card, please perform the following steps to increase your shader cache size:
1. Open your `NVIDIA Control Panel`
2. Click on `Manage 3D settings`
3. Scroll down in `Global Settings` until you see `Shader Cache Size`
4. Double-click `Driver Default` to the right and set it to `10 GB`
5. Click `Apply` and exit the application

![Shader Cache](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

#### Steam Setup

Nordic Souls only works with the Steam version of Skyrim. Additionally, it will only work with English versions of the game. While this may be understandably frustrating for users with different game versions or non-English speakers, there are major differences between game versions and I am only able to support one language.

A non-English version of the game will cause problems later. To verify that your game is in English, please perform the following steps:
1. Right click on Skyrim in Steam
2. Click `Properties`
3. Under `General`, set `Language` to `English`

> [!WARNING]
> If your Steam library is in Program Files, refer to [this](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) guide to move it elsewhere. Do not install do default Windows folders (Desktop, Documents, Downloads, etc.) as this will cause issues.

> [!CAUTION]
> There is no workaround for a pirated copy of Skyrim, or pirated Creation Club content. If you ask for support with anything pirated, you will be banned.

#### Installing CC Content

If you have not bought the Anniversary Edition DLC before, please do so. The list will not install without it. 

> [!WARNING]
> You should not verify file integrity through Steam. This will cause the wrong version of the Rare Curios creation to download, causing the installation to fail.

If you have Anniversary Edition and a fresh copy of Skyrim installed, and have yet to install Creation Club content, please perform the following steps:
1. Launch the game from Steam, and ignore any pop-ups about settings in the launcher. Run the game to get to the title screen.
2. You should receive a prompt to download all CC content, accept it.
3. Wait for the download process to complete. **This may take a while. Do not ALT-TAB during this process.**
4. When complete, close Skyrim.

### List Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://www.wabbajack.org/) and place it in a folder near or at the root of your drive, such as `C:\Wabbajack`. **Do not place it in Program Files, or in any default Windows folders like Desktop or Downloads.**

#### Downloading and Installing the List

Downloading and installing Nordic Souls can take a long time depending on your internet connection and PC specs. I recommend you install it on an SSD, as everything will go much faster. Complete the steps below for installation:
1. Create a folder near the root of your drive called `Nordic Souls`.
2. Open Wabbajack, go to `Browse lists`, find Nordic Souls, and click the download arrow. Alternatively, download the .wabbajack file from this repository or the [Nexus page](https://www.nexusmods.com/skyrimspecialedition/mods/77497), add it to your Wabbajack folder, and open it.
3. Set your installation folder to the folder you made in step 1 (e.g. `C:\Nordic Souls`).
5. Your downloads folder should be set automatically. If it isn’t, set it to either `Nordic Souls\downloads` or another location. It can even be on another drive.
6. Click the start button to begin. Follow any prompts on-screen. *Reiterating from earlier: if you do not have Nexus Premium, you will have to manually click through each mod. There are over 1100 mods.*
7. Wait. It may take an hour or more depending on your connection. Read the rest of the readme and take a nap. If you have any errors during installation, see below. Otherwise, carry on to [post-installation](#post-installation) when completed.

#### Problems with Installation

Some common errors you may encounter during installation:
- Could not download `X`:
  - Large files can fail to download due to connection issues. You can either run Wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads (`Nordic Souls\downloads`).
  - Make sure you have purchased the Anniversary Edition upgrade, and launched the game through Steam to download all CC content. Refer to [this section](#downloading-cc-content).
  - Try logging out of Nexus (in-app) and logging in again.
- `X` is not a whitelisted download:
  - This may happen when I update the list. Please check if there is a new update or wait if there is none.
- Wabbajack could not find the game folder:
  - You will never get support for a pirated copy of the game. Either buy the game *on Steam* or, if you did, go back to the [Pre-Installation](#pre-installation) section.
- Antivirus reports a virus:
  - Windows 10/11 may automatically quarantine a key file that is needed for MO2. You can fix this by [adding an exclusion for MO2 in windows defender](#antivirus-exceptions).
- Unable to download `Data_ccXXXXX - *.bsa` or `*.esp`:
  - Go back to [this section](#installing-cc-content) and make sure all CC content is installed. If it is, and you are on a legal copy of the game on Steam, then there is likely an error on Wabbajack or Bethesda's end and you will have to wait.
- Unable to download `Data_ccBGSSSE037-Curios - *.bsa` or `*.esl`:
  - This means you have verified integrity through Steam. You should delete them from `Steam/steamapps/common/Skyrim Special Edition/Data`, open the game through Steam, and redownload the files through the pop-up.
- Unable to download `Skyrim_Default.ini`:
  - Go back to the [this section](#steam-setup) section and change your game language to English.

If you are still having issues, visit the [Wabbajack Discord](https://discord.com/invite/wabbajack) or [my server](https://discord.com/invite/9cRs3KPyuW). **Please do not ask for support before going through the above steps and reading the [FAQ](https://github.com/Geborgen/nordic-souls/blob/main/FAQ.md).**

## Post-Installation

### Stock Game and Root Builder

Nordic Souls uses the [Stock Game](https://github.com/The-Animonculory/Modding-Resources/blob/main/Stock%20Game%20Setup.md) method. This is essentially a copy of Skyrim included with the installation folder. This means that everything is completely separate from your Steam installation of Skyrim (which is still required as the game files are not redistributed). The folder in question is called `Game Root`, located at `Nordic Souls\Game Root`.

The list also uses [Kezyma's Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720) to keep the game root folder clean. Any mod that needs to be installed in the game folder is instead added to MO2 with a special file structure, and is then added to the game folder whenever the game is running.

### Antivirus Exceptions

Generally speaking, using Windows Defender is advised as it is a solid antivirus software that will have minimal interference with the game. Antivirus programs can be notorious for false flagging MO2's VFS as problematic, causing crashes or other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will very likely need to fully remove them from your PC in order to actually launch the game through MO2.

If you use Windows Defender, it is advised that you set up an Exception for the modlist. Please follow these steps:
1. Press the Windows key, type `Windows Defender` in the search bar and select `Windows Security`.
2. Click on `Virus & threat protection` in the left pane.
3. Click the `Manage settings` option under `Virus & threat protection settings`.
4. Scroll down to `Exclusions` and click `Add or remove exclusions`. Accept the run with administrator prompt.
5. Click the `Add an exclusion` button at the top and choose `Folder`.
6. Navigate to your installation folder for the list and click `Select Folder`.

### Customizing the List

**Other than what is mentioned here, modifying the list in any way will void all support.** I cannot guarantee that everything will work if you add or remove mods. If you do add mods that include plugins, they must load **above** `Water for ENB (Shades of Skyrim).esp`. The paper map plugins should always be at the very bottom of your load order.

As this may cause some confusion, I should clarify that I'm not against people editing the list. All I mean is that I won't be able to help if things break. This also falls under Wabbajack's "rule 11", meaning that any modifications you make, you do so at your own risk. Visit the [modification guide](https://github.com/Geborgen/nordic-souls/blob/main/MODIFICATIONGUIDE.md) for more information.

Game settings and mod configs can be found in the `NS - Game Settings` mod under the `General Settings` separator in MO2. Right-click, open in explorer, and find the config you need, or click `Information...`, click the `INI Files` tab, and find what you need there. *If you're trying to configure a mod and it's not working, chances are it's being overwritten by a file from this mod.*

#### Optional Files

Under the `Optional Files` separator, you can enable and disable things to your liking. 

If you enable [ENB Frame Generation](https://www.nexusmods.com/skyrimspecialedition/mods/144507),  please read the mod page for more information and to determine if your system is compatible. All required settings have been preconfigured, you just need to enable the mod and enable it in-game under the ENB menu if needed.

#### ENB

Nordic Souls uses the tried-and-true [Rudy ENB](https://www.nexusmods.com/skyrimspecialedition/mods/4796).

If your interiors are too dark, edit `AmbientLightingIntensityInteriorDay` and `AmbientLightingIntensityInteriorNight` under the `ENVIRONMENT` category in the ENB menu.

If you want to add a different preset, you should familiarize yourself with [Kezyma's Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720), and match the way I've installed Rudy to MO2. This is unsupported.

If you do not want to use ENB, keep it toggled off in-game or switch to the Community Shaders profile.

> [!TIP]
> In-game, press `F10` to toggle the FPS counter, `SHIFT + ENTER` to open the ENB configuration menu, `SHIFT + INSERT` to toggle ENB, and `F7` to take a screenshot.

#### Community Shaders

Nordic Souls includes a separate profile for [Community Shaders](https://www.nexusmods.com/skyrimspecialedition/mods/86492). This provides a different aesthetic, and a customizable modular approach to shader effects. Performance is roughly the same as ENB.

To use Community Shaders, switch to the `Nordic Souls - Community Shaders` profile using the drop-down menu located in the top of the left panel in MO2. 

If you switch profiles mid-save, you will get a popup warning about missing plugins. You can safely ignore this.

> [!TIP]
> In-game, press `F10` to toggle the performance overlay, `END` to open the CS configuration menu, and `INSERT` to toggle CS.

#### Widescreen Support

Enable mods under the `Widescreen Support` separator.

#### Gamepad Support

Enable `NS - Gamepad Controlmap` under the `Gamepad Support` separator.


<details><summary>Gamepad Bindings (expand)</summary>

### Default Gamepad Bindings

![Gamepad Bindings](https://raw.githubusercontent.com/Geborgen/nordic-souls/refs/heads/main/.github/gamepad.png)

Sprint and dodge are mapped to the same button. Tap it to dodge, or press and hold to sprint.

Note that dodge will only work if you have the required perk. See the [gameplay guide](https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md).

You can press `F11` in-game to access this menu at any time.

</details>

#### Performance Tweaks

Nordic Souls should run fine on almost any machine, but there are some things you can do to improve performance if you're struggling:
- BethINI: Close MO2, open your installation folder, open `Tools`, open `BethINI`, run the program.

<details><summary>BethINI Settings (expand)</summary>

  ### BethINI Performance Settings
  - First make sure your paths are correct in the `Setup` tab: Game path should be `Nordic Souls\Game Root` and Mod Organizer should be your Nordic Souls folder. INI path should be `ModOrganizer > Nordic Souls - ENB` or `ModOrganizer > Nordic Souls - Community Shaders` depending on your desired profile.
  - On the `Basic` tab, check `Recommended Tweaks` and then `Medium`. Disable `VSync`. Make sure your monitor's resolution matches.
  - Set `Antialiasing` to `None`. This can cause weird shimmering in-game, however.
  - On the `Detail` tab, set `Godrays` to `None`. Set `Particles` to `2000`. Disable `Lens Flare` and `Anamorphic Lens Flare`. Set `Detailed Draw Distance` to `2000` and `Exterior Draw Distance` to `6000`. Disable `Ambient Occlusion`.
  - On the `View Distance` tab, set `Grass Fade` to `10000`, set `Level 8` to `32768`, and `Level 16` to `200000`.
  - Go back to the `Basic` tab, click `Save and Exit`.

  Thanks to [Elysium Remastered](https://github.com/TitansBane/Elysium-Remastered) for some of these tweaks.
  
</details>

- ENB: Toggle ENB with `SHIFT + INSERT`. Completely removing ENB has caused issues for users, so keep it disabled instead.
- ENB: Press `SHIFT + ENTER` to open the ENB menu, untick `EnableAmbientOcclusion` under `Effect` in the left column, and then `---SAVE CONFIGURATION---` at the top.
- ENB: Enable the `ENB Frame Generation` mod under the `Optional Files` separator. Please note that unless you can get a high FPS without it and have a monitor with a high refresh rate, it won't do much for you.
- CS: Press `END` to open the CS menu, scroll down to Light Limit Fix, click `Disable at Boot` on the top right, then go to Screen Space GI and do the same; save on the top right.
- CPU Priority: [Skyrim Priority](https://www.nexusmods.com/skyrimspecialedition/mods/50129) is included to elevate CPU priority, but you need to use an [included tool](https://www.nexusmods.com/skyrimspecialedition/mods/94636) to set CPU affinity. Click the Tools (puzzle piece) icon on the top left menu in MO2, click `Set CPU Affinity`, and click `OK`. If your affinity is already set, keep it enabled.
- External tool: [VRAMr](https://www.nexusmods.com/skyrimspecialedition/mods/90557). Watch [this](https://www.youtube.com/watch?v=MS8vhuyeT2g) video for more information. This falls under modifying the list, meaning you are responsible for potential issues that may arise.
- Pay to win: upgrade hardware. SSD will improve load times, RAM will reduce stuttering, GPU and CPU will increase performance. This isn't a PC guide, there are plenty of those on the internet.
- Pay to win:  [Lossless](https://store.steampowered.com/app/993090/Lossless_Scaling/). It acts as an upscaler, and also includes framegen. You can try it, and since it's on Steam, if it doesn't work for you, you can refund it within two weeks if you use it for less than two hours.

#### Modification Guide

Modifying the list in any other way is unsupported, but not unwelcome. Visit the [modification guide](https://github.com/Geborgen/nordic-souls/blob/main/MODIFICATIONGUIDE.md) for more information.

## Playing the List

### Starting Up

Open the installation folder and open `ModOrganizer.exe`. Make sure the dropdown box on the right is set to `Play Nordic Souls` and run it.

> [!TIP]
> You can create a desktop shortcut in the shortcuts dropdown.

> [!CAUTION]
> Do not launch the game through Steam directly. This will launch vanilla Skyrim.

> [!TIP]
> If you want to launch the game through Steam, Big Picture included, do the following:
> 1. Right click on Skyrim in your Steam Library and select Properties.
> 2. In Launch Options command line add the following:
>    
> ```"C:\Games\NordicSouls\ModOrganizer.exe" "moshortcut://:Play Nordic Souls [SKSE]" %command%```
> 
> Naturally, path to .exe should be matching your own. You can copy it from shortcut from the tip above.
> 
> For Big Picture, you may want to re-enable in-game overlay. Don't use it to exit the game though, it will stuck; use in-game menu instead.

> [!CAUTION]
> Do not "unlock" MO2 when the game is running. This will cause various issues within the game.

#### Controls

<details><summary>Key Bindings (expand)</summary>

### Default Key Bindings

![Key Bindings](https://raw.githubusercontent.com/Geborgen/nordic-souls/refs/heads/main/.github/keyboardandmouse.png)

Any key highlighted in green has `SHIFT` as a modifier (e.g. `SHIFT + ENTER` for the ENB menu).

Sprint and dodge are mapped to the same button. Tap it to dodge, or press and hold to sprint. Dodge also has a second mapping on the mouse, as seen in the above image.

Note that dodge will only work if you have the required perk. See the [gameplay guide](https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md).

You can press `F11` in-game to access this menu at any time.

</details>

Refer to [this section](#gamepad-support) for gamepad setup and controls.

### Mod Configuration Menu

MCMs have been pre-configured. Wait until you receive a "configuration complete" pop-up (you can ignore messages in the corner, as they appear slower than everything actually loading). Afterwards, you can tweak them to your liking if you want to customize your experience.

### Starting the Game

Character creation has been overhauled. High Poly Head is selected automatically. Nordic Souls includes several character presets for you to choose from, but you can easily add your own.

You will spawn in a cell. **Wait until you see a "configuration complete" pop-up** before continuing. If you wish to edit your character again, you can activate the Runic Stone located on the wall near the door. Otherwise, interact with the Statue of Azura to select your starting point. You can go through the vanilla intro sequence if you want, but I recommend exploring all the options.

Once you've selected your start, activate the Arcane Circle on the floor to enter the world.

You can activate the Select Traits power in your magic menu to select up to two unique character building traits, if you so wish.

### Gameplay Guide

The gameplay guide can be viewed [here](https://github.com/Geborgen/nordic-souls/blob/main/GAMEPLAYGUIDE.md). It includes a more in-depth explanation of what the list is actually trying to do, along with breaking down the different gameplay overhauls, quest mods, and other mods to pay attention to.

### Note for Content Creators

Some of the added music in the list cannot be played on YouTube/Twitch or other platforms due to DMCA rules. To circumvent this, I recommend disabling in-game music with the audio slider.

## Updating the List

Before updating, please check the [changelog](https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md) and back up your saves. You may need to start a new save after certain updates, this will be indicated in the changelog.

Updating is like installing the list. Just make sure your paths are the same.

> [!WARNING]
> Any changes you have made to the list will be reverted upon updating. To keep mods that you added, prefix the mod name with `[NoDelete]`.

## Uninstalling the List

Simply delete the folder, and you have uninstalled the list.

## Known Issues

Please refer to the [issues](https://github.com/Geborgen/nordic-souls/issues) tab before reporting an issue. Additionally, common bugs will be discussed on Discord. 

Keep in mind that although I try to fix issues as they come up, I cannot fix everything. Additionally, please be patient with support, as this is a hobby and schedules may be different.

If your issue isn't listed, see below.

## I found a bug!

Visit the [issues](https://github.com/Geborgen/nordic-souls/issues) tab to see if your issue was already reported. If not, create a new issue. Please be as detailed as possible, and use the template provided.

## Changelog

To see the changes and version history, visit the [changelog](https://github.com/Geborgen/nordic-souls/blob/main/CHANGELOG.md).

## FAQ

Please refer to the [FAQ](https://github.com/Geborgen/nordic-souls/blob/main/FAQ.md) before asking for support.

## Credits and Thanks

- YOU for reading this.
- All mod authors for their hard work.
- Halgari and the Wabbajack team for making this awesome tool.
- Other Wabbajack list authors for their help and inspiration and answering all my questions.
- The community helpers and moderators in my Discord server for their amazing assistance with ideas, testing, and community support.
- The beta testers who helped make the list the best it can be.
- Everyone who has played the list that has helped in some way, by finding issues and contributing ideas.
- Based Department (you know who you are).

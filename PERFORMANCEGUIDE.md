# Gameplay Guide

Despite Nordic Souls being relatively performance-friendly, it can still be taxing on low-end systems. There are several things you can do to decrease stuttering and increase overall performance.

## Contents
- [Hardware Upgrade](#hardware-upgrade)
- [ENB](#enb)
- [BethINI](#bethini)
  - [Basic Tab](#basic-tab)
  - [Detail Tab](#detail-tab)
  - [View Distance Tab](#view-distance-tab)
- [SSE Display Tweaks](#sse-display-tweaks)
- [Upscaler](#upscaler)
- [LOD](#lod)
- [Wrapping Up](#wrapping-up)

## Hardware Upgrade

In no way do we recommend spending this type of money if you are not in a financially comfortable situation, but if you have a flexible budget, it might be worth looking into. This is not a PC guide, so this section will be brief.

The first thing you should look into for PC upgrades is storage. The switch from a hard disk to a Solid State Drive (SSD) or SSD to NVMe is incredible. Everything will load noticeably faster and with minimal stuttering. Secondly, your graphics card, or GPU, while easily one of the most expensive parts of your PC, will cause drastic differences. Of course, it's also worth investing in more/faster RAM and a higher-end CPU. Again, this isn't the guide for PC hardware, but if you have the money then it's something to think about.

## ENB

Nordic Souls includes 12 total ENB presets for you to choose from. Some are more performance-friendly than others.

Open ENB Organizer (dropdown at top right of MO2), ignore any warnings about Nexus updates, click the three bars on the top left, and navigate to the presets tab.

From there, you will see the ability to toggle several ENB presets. For the best performance, select iiENB or Weather Is Sacred ENB.

*The ENBs that say "performance" aren't necessarily performance-friendly compared to other ENBs. They are just performance-friendly compared to the ENB that they are the performance version of.*

**Make sure you only have one ENB enabled at a time.**

[Here is a higher-quality comparison of all the included presets.](https://imgur.com/gallery/3WDkZit)

Completely disabling ENB is not recommended, as users have had issues with it. Press `F12` to toggle it in-game.

## BethINI

BethINI comes pre-packaged with the list. To open it, **close MO2** and navigate to `[YOUR INSTALLATION FOLDER]\Tools\BethINI`.

Once you open BethINI, you should first go to the `Setup` tab and make sure your pathing is correct. The game path should be the Stock Game folder and the INI path should be the Nordic Souls folder. [This is what mine looks like.](https://user-images.githubusercontent.com/88332109/227602080-c1e05e4f-e880-46eb-913a-1dad845de523.png)

### Basic Tab
- Check `BethINI Presets` and `Recommended Tweaks`, then `Medium` or `Low`.
- Uncheck `VSync` and `Lock Frame Rate`.

### Detail Tab
- Sset `Decal Quantity` to `Medium` or `Low`.
- Set `Godrays` to `Medium`, `Low`, or `None`.
- Set `Shadow Resolution` to `1024` or lower.
- Disable `Ambient Occlusion`.

### View Distance Tab
- Set `Grass Fade` to `10000` or lower.

Back on the `Basic` tab, save and exit.

## SSE Display Tweaks

The [SSE Display Tweaks](https://www.nexusmods.com/skyrimspecialedition/mods/34705) has quite a lot of configuration options, but most of them are disabled by default.

To find the INI, open the `WRAPPING UP - OUTPUT` separator in MO2. right-click the `[NoDelete]NS - Game Settings` mod, and click `Information...`. Find the `INI Files` tab and find `SKSE\Plugins\SSEDisplayTweaks.ini`.

- Set `#Fullscreen=false` to `Fullscreen=false`
- Set `Borderless=false` to `Borderless=true`
- Set `BorderlessUpscale=false` to `BorderlessUpscale=true`
- Set `#Resolution=1920x1080` to `Resolution=[YOUR MONITOR RESOLUTION]`
- Set `#ResolutionScale=0.75` to `ResolutionScale=0.9`

Remeber to remove the `#` where noted, so the tweaks actually work. The minimum you should set the resolution scale to is `0.8` or you may have a blurry game.

## Upscaler

Skyrim now has support for upscaling, using technology like [DLSS](https://www.nvidia.com/en-us/geforce/technologies/dlss/), [FSR2](https://www.amd.com/en/technologies/fidelityfx-super-resolution), and [XeSS](https://www.intel.com/content/www/us/en/products/docs/arc-discrete-graphics/xess.html).

Get the base plugin from [here](https://www.nexusmods.com/site/mods/502). You can then read [the mod page](https://www.nexusmods.com/skyrimspecialedition/mods/80343) for installation instructions, but keep in mind that this version *does not work with ENB*. If you want to use ENB with the list, you will need the version from [PureDark's Patreon](https://www.patreon.com/PureDark). At this time, you will have to pay, but it will be released to the public eventually.

You won't recieve support for adding the upscaler because it falls under modifying the list.

## LOD

Nordic Souls uses relatively performance-friendly LODs, but they can still cause stuttering on low-end computers. Thankfully, they can be disabled or re-generated.

To disable the LODs, open the `WRAPPING UP - OUTPUT` separator and disable `NS - xLODGen Output`, `NS - TexGen Output`, and `NS - DynDOLOD Output`. If you re-enable these, refer to the plugin placement [here](https://loadorderlibrary.com/lists/nordic-souls).

You can also re-generate the LODs at a lower quality. Plese note that this now falls under Wabbajack's rule 11 and you will not recieve support if you break things.

All the tools you need are included. In MO2's application drop-down, click `<Edit...>`. Find `xLODGenx64`, `TexGenx64`, and `DynDOLODx64`. For each application, disable `Hide in user interface`.

Please refer to [Althro's DynDOLOD guide](https://github.com/The-Animonculory/Modding-Resources/blob/main/DynDOLOD.md) when generating LODs. You can skip steps involving Grass LODs (unless you want to generate grass cache and do it yourself) and ACMOS (NS uses a paper map). Some things you can do are disable 3D tree LODs and use DynDOLOD low rules.

[For reference, these are the settings that NS uses by default.](https://imgur.com/gallery/sTF2mBr)

## Wrapping Up

This should help performance, at least a little bit. If none of these tweaks work for you, refer to [this step](#hardware-upgrade).

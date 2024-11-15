# FAQ

## Q: Do I have to read this?

**A:** No, but if you ask a question that is in this document, you will likely be referred here.

## Q: Why does my character look broken and glitchy?

**A:** You unlocked MO2 when launching the game. When you get the pop-up after launching, do not unlock. This will unload files, causing strange issues.

## Q: My game crashes as soon as I try to launch it.

**A:** Reinstall the list to verify any missing/broken files. If you still have issues, go back and make sure you have all prerequisits (.NET, etc.). Install them even if you think you have them. **Make sure you have disabled OneDrive.**

## Q: Why is my game window super zoomed-in?

**A:** Go to your `Game Root` folder, right-click `SkyrimSE.exe`, go to `Properties`, and follow the steps outlined [here](https://raw.githubusercontent.com/Lost-Outpost/resources/main/skyrim-scaling.png).

## Q: Why is my map purple/missing?

**A:** You have a plugin loading below the paper map plugin. Either reinstall the list to restore the load order, or refer to the [modification guide](https://github.com/Geborgen/nordic-souls/blob/main/MODIFICATIONGUIDE.md) if you've added mods.

## Q: How do I change my FOV?

**A:** first use the FOV console command like normal (`fov x x`) (yes, input the value twice).

## Q: How do I change my brightness?

**A:** In the ENB menu, go to the `ENVIRONMENT` category, and edit settings such as `AmbientLightingIntensityDay` and `AmbientLightingIntensityNight`. You can also find settings for interiors, if interiors are too dark. If you break something, you can press `LOAD CONFIGURATION` at the top to restore your previous configuration, or reinstall the list to reset everything to default.

## Q: I've modified INI settings (e.g. as dodge hotkey), why are they not applying?

**A:** Check the `NS - Game Settings` mod. Modify the INI files there.

## Q: How do I get rid of those obnoxious category icons at the top of the inventory menu?

**A:** Enter the `SkyUI` MCM, go to `General`, change `Category Icon Theme` to `SkyUI V5`.

## Q: Where did my compass go?

**A:** Press `X` to toggle your compass.

## Q: How come I can't access this chest/steal this item?

**A:** You must be sneaking to steal items. You can configure this in the `Better Third Person Selection` MCM.

## Q: Why is the QuickLoot menu not showing up?

**A:** If a container has a large amount of items, the QuickLoot menu will no longer appear, in order to prevent crashing.

## Q: Why are dragons/other large creatures invisible?

**A:** If this bothers you, go to `SSEDisplayTweaks.ini`, find `DisableActorFade=false` and set it to `true`.

## Q: Why does this quest not start?

**A:** There are likely different starting requirements. Please refer to [this](https://github.com/Geborgen/nordic-souls/blob/main/QUESTCHANGES.md) document.

## Q: Why are no dragons spawning?

**A:** This is due to the [Diplomatic Dragons](https://www.nexusmods.com/skyrimspecialedition/mods/70803) mod. Random dragons will not spawn until Sahloknir dies.

## Q: Why am I missing health/regeneration? How do I get rid of injuries/infenctions?

**A:** Sleep for 4 hours to cure minor injuries, 8 for major, and 12 to cure critical/all injuries. Infections act as diseases, so use a cure disease potion.

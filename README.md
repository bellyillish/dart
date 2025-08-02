# Dynamic Aspect Ratio Tweaks (DART) for GAMMA

A bunch of (mostly UI) fixes for GAMMA. Primarily aimed at ultrawide users, but also includes features that can be useful to everyone. Fixes are modular and independent from each other, so you can disable individual ones if you need to while keeping the others active. Everything is dynamic and monkey-patched to make it as compatible as possible with other mods. It's focused only on the fixes and lets other mods add the fun stuff. DART is happiest when you forget it's even there.

DART also lets you customize various UI elements through MCM. You can move and scale the main HUD elements to your liking even if you're not an ultrawide user.

- [The Fixes](#the-fixes)
- [Other Notes/Tips](#notestipstroubleshooting)
- [Installation](#installation)
- [Configuration](#configuration)
- [Credits](#credits)
- [Links](#links)


## The Fixes

### Dart Core
Sets the stage by making sure ultrawide users get the best possible template for *every* UI element. Without DART the game assumes you are a 4:3 user and gives you outdated, crappy templates that nobody maintains. With DART you at least get the much better 16:9 templates. It also includes a "safe zone" MCM option to globally inset all HUD elements. It is required because it also includes shared code that the rest of DART uses.

### BHS HUD
Corrects the BHS HUD's width and position to your aspect ratio (i.e. makes him look less fat). You can also scale or move this element in MCM.

### Companion List HUD
Corrects the position and width of the HUD element that shows health bars and distances of your companions. It positions it so it's no longer partially off screen, but you can also manually move or scale it in MCM. It works with the minimalist version that ships with GAMMA and the more detailed Anomaly version used by some UI skins.

### Faction ID Patches HUD
Corrects the width and position of Faction ID patches when you hover over NPCs. It can also be moved or scaled in MCM. The Faction ID Patch mod includes its own (much more in-depth) settings to customize it. If you use both, DART will combine the two so they work together.

### Status Icons HUD
Corrects the positions between and around the status icons. You can scale, move, or adjust the spacing between icons in MCM.

### Messages List HUD
Corrects the size and position of News Manager messages. You can scale or move this element in MCM. Note that it's not possible to scale text the same way as other graphical elements, so the scale setting will only adjust the size of thumbnails and the overall space used by messages.

### PDA Map Markers
Fixes the widths, positions and alignments of all icons in the PDA and minimap. At least as much as it can -- for example you may notice the diagonal arrows for level transitions will still look a little wonky (especially in 32:9). This module doesn't have any MCM settings.

### PDA Font Sizes
Tries its best to make fonts more legible in the 3D PDA for ultrawide users. Since text can't be scaled, this is an imperfect but as-good-as-I-can-do solution. The game includes only a handful of predefined font sizes. This module allows you to uniformly bump up the font size for all text elements by up to 3 sizes. It also lets you choose a maximum size "cap" to prevent the largest fonts from getting *too* big.

### Minimap & Compass
Fixes the broken layouts of the circular and square minimaps. You can scale, move, adjust the opacity, and realign the map to any side or corner of the screen in MCM. You can also move the clock (in the circular minimap only). This module is  compatible with the "Compass Only" mod, but you may need to manually adjust its position in MCM depending on the alignment you choose. You can even emulate the compass-only look with the other minimaps and the right combination of settings.

### Ammo & Companion Wheels
Fixes the widths and positions of the ammo and companion wheels. You can scale and move each in MCM. You can also choose to use the round ammo wheel instead of the triangular one in MCM.

### Inventory Icons
Lets you adjust the scale of and spacing between inventory icons in MCM. Also automatically tweaks the size of these icons to fill the available space and prevent them from getting cut off in the UI. Note that the spacing setting is experimental and can cause icons to get cut off anyway. Leaving it at 0 will minimize this.

### Ammo Type HUD
This is for a relatively obscure but good little mod. If you haven't installed this mod on your own then you don't need this module. If you did, it will fix the position of the ammo type text so it doesn't overlap the BHS HUD.


## Notes/Tips/Troubleshooting

### If the map looks stretched vertically in the 3D PDA...
Unfortunately this is a bug in the game engine and can't be fixed at the mod level. If you're a 21:9 user (like me) you can probably get used to it pretty quickly. If you're a 32:9 user however it's a lot more annoying. Many 32:9 players use the 2D PDA instead.

### If text is unreadable...
This is another game engine bug very similar to the one above. It is particularly bad on 32:9 as the text is squished horizontally to the point of illegibility. If DART's PDA font size fixes aren't enough, try activating the 2K or 4K Tactical Fonts that come with GAMMA (mods 309 & 310).

### If you feel like you're playing in a fishbowl...
You need to adjust the FOV in "Settings" -> "Visual Settings" -> "Basic". There are 2 settings: "FOV" and "HUD FOV". Make the "FOV" smaller until it feels right -- there's no right answer, it's subjective. I don't know **exactly** what "HUD FOV" does but I've generally heard to leave it at 65.

### If you have issues going through doorways or bumping into things...
See above about "FOV".

### If your game freezes while loading a save after installing DART...
As of writing this (2024.12.04), the 11/30 modded EXEs cause many freezes, and this is one of them. If you've updated your modded EXEs on your own, replace them with an earlier version or revert to the ones that come with GAMMA.

### If you see cutoff icons in other places beside the inventory...
There are a lot of things that DART doesn't fix yet because each needs its own fix written specifically for it. This particular issue is at or near the top of the list, but dealing with these icon grids is complicated.

### If you want to use the square minimap or only the compass, but it's not working as expected...
Make sure you follow the directions in Discord for enabling these or else they won't work right: https://discord.com/channels/912320241713958912/976570969768476753/1152662325296382172

## Installation

1. Go to [releases](https://github.com/bellyillish/dart/releases) and download the latest one at the top of the list. DO NOT CLONE OR DOWNLOAD THE SOURCE FILES DIRECTLY or you will have a bad time.
2. Install it with Mod Organizer 2 (included with GAMMA): https://anomalymodding.blogspot.com/2021/04/Mod-Organizer-2-setup-and-Amomaly-modding-guide.html
3. In most cases you can leave the checkboxes as-is when prompted (they should all be ticked except one). If you have another mod that touches one of the UI elements above and DART conflicts with it, untick the offending module. If you've installed the Ammo Type HUD mod, tick the box for that.
4. Priority won't matter most of the time as long as it's below the mods that come with GAMMA, but if you want to be extra safe keep it towards the bottom of the list.


## Configuration

Head over to "Mod Configuration Menu" -> "DART" to change settings. They are organized by module.


## Credits

- Thanks to @nomotion who contributed to many of the HUD fixes and features, and joined me in banging my head against the wall from time to time. He also made a nifty automated release workflow in GitHub.

- Thanks obviously to @b0nesy and his crew for GIRTH. This was my first mod and I wouldn't have been able to do any of it without having GIRTH to reverse engineer and study.

- Thanks obviously to @grokitach and the GAMMA crew. I've barely touched my Steam backlog in almost a year thanks to this awesome game.


## Links

- Discord: https://discord.com/channels/912320241713958912/1169311822139105380/1169311822139105380

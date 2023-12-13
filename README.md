# Dynamic Aspect Ratio Tweaks (DART) for GAMMA
A collection of fixes for ultrawide displays (21:9, 32:9, etc.). Each fix is modular, independent, and can be enabled/disabled as you prefer. Fixes are script-based and adapt to existing code, resulting in better compatibiltiy and fewer conflicts. They are also dynamically calculated based on your aspect ratio, so they will work equally well for any resolution wider than 16:9.

DART wants to be minimal, unopinionated, and focused only on ultrawide fixes. It tries to lay a foundation upon which you can customize with additional mods. It is regularly tested with UI Rework, EGUI, DynaHUD, and a few other UI-customization mods.

DART is customizable via a config file that allows you to move and scale various UI elements to your liking. It also includes a "safe zone" setting to inset UI elements from the edge of the screen if you'd like. A planned migration from a config file to MCM is planned for a future version.

## List of Fixes:
- Ensures that ultrawide users get served the correct XML file: 21:9 if it exists, then 16:9 if it exists. This should give you a somewhat-improved experience across the board (instead of old and neglected 4:3 templates that are inferior to what 16:9 users get).
- Circular minimap that can be repositioned and scaled. The clock can be moved as well. A combination of settings can give you a compass-only look.
- Un-squished markers and icons on the PDA, and properly-aligned highlights/indicators on both the PDA and minimap.
- Size adjustments to avoid partially cutoff inventory icons. Icons can be resized.
- Un-stretched ammo and companion wheels.
- Global fix for 2D scopes. This fix can replace the ones included in GAMMA. If authored correctly, scopes added by mods should automatically be detected and fixed.
- Fixed proportions and positions of HUD elements (BHS, faction ID patches, status icons, messages list, companion list).
- Mask fixes ported from GIRTH (with permission).

## Installation:
Install with MO2. Choose "00 Dart Core (Required)" plus any/all fixes during installation. The safest place to install is at the bottom of load order, but in most cases priority won't matter.

- Get v2.0 here: https://discord.com/channels/912320241713958912/1169311822139105380/1184634823889920141
- GitHub: https://github.com/bellyillish/dart
- Discord: https://discord.com/channels/912320241713958912/1169311822139105380/1169311822139105380

## Configuration:

Once installed, look for /gamedata/scripts/dart_config.script, which has an annotated list of possible configuration options. These values are tweaked for a vanilla GAMMA experience, and you may want to make your own adjustments if you're using a third-party UI mod.

## Credits:

- Special thanks to @nomotion who contributed to many of the HUD fixes and features, and joined me in banging my head against the wall from time to time. He also made a nifty automated release workflow in GitHub.

- Thank you obviously to @b0nesy and his crew for GIRTH. You blazed a trail that provided a roadmap for a n00b like me. Start here:  ⁠╟📎mods-posting⁠GIRTH - Ultrawide Fixes, and scroll through and appreciate the hard work, collaboration, and trial and error that went into it.

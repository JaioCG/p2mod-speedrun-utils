# Portal 2 Mod SAR Categories

[SourceAutoRecord](https://sar.portal2.sr) speedrun categories for different Portal 2 mods.

SAR supports a couple of mods' timing categories by default, however the majority of them need to be added manually. Instead of having these categories strawn about the internet, I've decided to collect as many as I can here.

SAR already supports categories for Portal 2, Aperture Tag, Portal Stories: Mel, Thinking with Time Machine, and Portal Reloaded. These won't be included here.

## Installation

1. Open `cats.md` and search for the mod you wish to create a category for.
2. Copy the lines containing "sar_speedrun_cc_" and paste them into a new `.cfg` file that'll hold category definitions.
   1. **NOTE: Many of these categories are already included with srconfigs, and do not need to be added into a custom categories file. Check `srconfigs/mkcats.cfg` to see if the category is already included.**
   2. Remember to add `exec custom_cats` (or whatever you decided to name the file) in your `extra.cfg` (or autoexec if you don't use srconfigs).
3. Create a new `.cfg` file for the specific mod's recording/category set commands, or download the Demo Category (read below) to use as a base.
   1. srconfigs users should put this file in `srconfigs/cats`.
4. Add the "sar_speedrun_category" and "sar_alias do_reset" lines to this new file.
   - Feel free to change the `map` part of the do_reset alias to be a save loading if the mod has a vault/start save available.
5. If you use srconfigs, add "add_cat [mod file name]" to your `extra.cfg` file, and in-game, run `[mod file name]` to load the category.

## Demo Category

For those that don't want to create a new config file from scratch for a mod, I've included a `demo-category.cfg` file that contains most of the commands needed for a run, including demo recording commands. The file is based on srconfigs' category files, however it does work standalone.

To install, download the file and follow the included instructions to set up. This file is meant to be the "specific mod file" mentioned in Step 3 of the installation guide above.

*Do note that some mods use different proof standards, so you may need to edit some of the demo recording and timing commands.*
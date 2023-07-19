# Portal 2 Mod SAR Categories
[SourceAutoRecord](https://sar.portal2.sr) speedrun categories for different Portal 2 mods.

SAR supports a couple of mods' timing categories by default, however the majority of them need to be added manually. Instead of having these categories strawn about the internet, I've decided to collect as many as I can here.

SAR already supports categories for Portal 2, Aperture Tag, Portal Stories: Mel, Thinking with Time Machine, and Portal Reloaded. These won't be included here.

## Installation
1. Open `cats.md` and search for the mod you wish to create a category for.
2. Copy the lines containing "sar_speedrun_cc_" and paste them into the mod's `.cfg` file
   - If you're using [srconfigs](https://github.com/p2sr/srconfigs), put these commands into the `mkcats.cfg` file.
3. Add the "sar_speedrun_category" line to the mod's `.cfg` file and set it to the category you want to use. srconfigs users should put this file in the `cfg/cats` directory.
4. Add the "sar_alias do_reset" line to the end of the mod's `.cfg` file. This command is used to stop and reset a run.
   - Feel free to change the `map` part of the do_reset alias to be a save loading if the mod has a vault/start save available.

## Demo Category
For those that don't want to create a new config file from scratch for a mod, I've included a `demo-category.cfg` file that contains most of the commands needed for a run, including demo recording commands. The file is based on srconfigs' category files, however it does work standalone.

1. Download this file, place it in `cfg/cats` (or just cfg without srconfigs), and rename it to the mods name.
2. Follow the instructions on the file to set up the category.
3. [SRCONFIGS ONLY] Add the command `add_cat <file name>` to your extra.cfg file. Then in game, you can run `<file name>` to select the category.

*Do note that some mods use different proof standards, so you may need to edit some of the demo recording and timing commands.*

## Contributing
For any new mods added to [speedrun.com](https://github.com/p2sr/srconfigs), please put in a pull request here with the mod's SAR category. If you're not sure how to do this, feel free to ask in the [SAR Discord](https://discord.gg/p2sr).

## Todos
- Add offset times for mods that have a vault save
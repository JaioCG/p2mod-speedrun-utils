# Portal 2 Mod SAR Categories
[SourceAutoRecord](https://sar.portal2.sr) speedrun categories for different Portal 2 mods.

SAR supports a couple of mods' timing categories by default, however the majority of them need to be added manually. Instead of having these categories strawn about the internet, I've decided to collect as many as I can here.

SAR already supports categories for Portal 2, Aperture Tag, Portal Stories: Mel, Thinking with Time Machine, and Portal Reloaded. These won't be included here.

## Installation
1. Open `cats.txt` and search for the mod you wish to create a category for.
2. Copy the lines containing "sar_speedrun_cc_" and paste them into the mod's `.cfg` file
   - If you're using [srconfigs](https://github.com/p2sr/srconfigs), put these commands into the `mkcats.cfg` file.
3. Add the "sar_speedrun_category" line to the mod's `.cfg` file and set it to the category you want to use. srconfigs users should put this file in the `cfg/cats` directory.

## Contributing
For any new mods added to [speedrun.com](https://github.com/p2sr/srconfigs), please put in a pull request here with the mod's SAR category. If you're not sure how to do this, feel free to ask in the [SAR Discord](https://discord.gg/p2sr).
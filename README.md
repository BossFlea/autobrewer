# Hypixel Skyblock autobrewer
This repository acts as the place to download all the schematics for my Hypixel Skyblock autobrewer(s) and learn how to use the them! All schematics are for [Litematica](https://www.curseforge.com/minecraft/mc-mods/litematica) (obviously the brewer is designed for Hypixel's 1.8.9 and has been thoroughly tested, I've used this brewer to brew over 1500 splashes as of June 2024). I recommend downloading litematica on the newest supported minecraft version (currently 1.20) and building the brewer on hypixel using this version.

*Make sure to read the tips and instructions on this page, especially the `How to use the autobrewer` section!*

### June 2024 Schematics Update:
This update brings new, updated schematics for all the brewer variants, notably including the new Cold Resistance potion, as well as an optimised output system, making it both much easier to build and considerably faster to retrieve a splash. This removes the need for seperate schematics with rainbow output capabilities, as it is now just as easy to build. The new schematics also include a few miscellaneous improvements that should help with the overall reliability of the brewer.
- I've made seperate schematics that can be used to upgrade the output system of an existing brewer, these can be found [here](upgradeschematics), with a seperate one for the 'small' brewer variant. (*Make sure to correctly align the schematic, this is easiest by the line of droppers!* You also don't have to break any of the chests/hoppers, meaning the storage does *not* need to be empty for this change) Please note that these update schematics only include the new output system, if you'd like to have the Cold Resistance potion, among other things, you will have to get one of the full schematics.

In addition to this, there is also a new [Money efficient variant](https://github.com/BossFlea/autobrewer#money-efficient-variant) of the brewer, which doesn't include any of the useless/broken potions that serve no purpose on bingo. This saves a lot of coins over time, while having no impact on anything.

If you have any problems or questions, feel free to dm me on discord or visit my island on skyblock! Discord: `bossflea`, ign: `BossFlea`

## Main bingo splashes brewer
### General features
- automatic input of awkward potions, xp boosts, spirit/mf etc.
- seperate brewer to automatically fill awkward potion storages
- brew up to 192 splashes in one batch without refilling the potion ingredients
- brews (coffee etc.) have to be put into the brewing stands manually due to Hypixel's mechanics (this is unavoidable with any system)
- average time per 1 splash can quite easily be under 20s from my experience (one half of a cycle takes ~20s, the other half includes putting brews in, ~35s. 55s/3=<ins>18.3s</ins> per splash)

<ins>**!! Important !!**</ins> The brewer will break if you don't open every brewing stand every time before starting a brewing session! If you reload your island, this gets reset. This is another issue caused by Hypixel and is unavoidable.
Tip: Do this at the same time as you're initially filling the ingredients into the brewing stands to save time

<details>
  <summary>❗<ins><i><b>(EXPAND)</b> How to use the autobrewer</i></ins></summary>
  
  - First make sure you have enough xp boosts, awkward potions (let the seperate brewer run for a while, also remember to manually transfer the night vision to the main brewer's invisibility input chests if you have the 36 pots variant), spirit/mf, wisp potions etc. in the input storage, as well as enough brews in the seperate brew dispenser.
    - I highly recommend using ooffyy's [Bingo+ pack](https://modrinth.com/resourcepack/bingo+) for its xp boost and awkward potion textures, which are extremely helpful!
  - Then fill your chosen amount of ingredients into the brewing stands, following the carpet color coding. Make sure to also click the brewing stands that don't need any ingredients or ones that may have already been filled previously!
  - Now to start brewing, you first need to make sure the `Enable Input` lever is on. If the `Move Potions` lever is in the correct state, the brewer should start filling the brewing stands in the top row. While this is happening, manually fill the brewing stands which require brews (Do this starting from the side with the levers to avoid problems).
  - Once all brewing stands are filled, click the `Move Potions` lever. The potions will start moving down to the next layer. These ~20s are a good time to refill the agility potion's top row brewing stand with an enchanted cake from the chest above and fill your inventory with a new set of brews for the next cycle (if you're using the 36 pots version, 1 item won't fit in your inventory, use stash or /ec).
  - When all the potions have finished moving down a layer, click the `Move Potions` lever again. Now repeat the last two steps until your ingredients run out.
  - To stop the awkward potions etc. from automatically being filled into the brewing stands when you want to stop brewing, set the `Enable Input` lever to off. You might also need to use this lever if the awkward potion input redstone gets stuck in the locked state while brewing.
  - Refer to [this graphic](https://i.imgur.com/mqz9NFB.png) to learn about how to retrieve splashes and in what order to splash them
    - *Make sure you don't forget any of the filler items visible in the graphic!!*
</details>

A visual guide for the brewer in the form of a video is coming soon™️

### [Large storage variant](mainbrewer)
- 36 potion splashes
- 6 double chests of output storage per potion (max 373 full splashes)
### [Medium storage variant](mainbrewer)
- 36 potion splashes
- 4 double chests of output storage per potion (max 255 full splashes)
### [Small storage variant](mainbrewer)
- 36 potion splashes
- 2 double chests of output storage per potion (max 137 full splashes)
### [Money efficient variant](mainbrewer)
- 26 potion splashes
- 2 double chests of output storage pet potion (max 137 full splashes)
- This variant lacks all the useless/broken potions that serve no purpose on bingo


## Alchemy 50 autobrewer (fully automatic)
### Variants
- [Enchanted Fermented Spider Eye](alchemy50)
- [Enchanted Sugar Cane](alchemy50) (can also be used for any other material that requires awkward potions, e.g. Enchanted Cookie)
### Features
- fully automatic: leave it running afk and claim the xp by emptying the storage through a brewing stand
- optional glowstone functionality for some money back by npc selling
- easy to build and easily extendable (1 block wide columns, more than ~3 columns is not recommended)

<ins>Warning!</ins> Make sure to click every brewing stand before starting the autobrewer! You also can't leave your island while the brewer is running

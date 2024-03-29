# Hypixel Skyblock autobrewer
This repository acts as the place to download all the schematics for my Hypixel Skyblock autobrewer(s) and learn how to use the brewers! All schematics are for [Litematica](https://www.curseforge.com/minecraft/mc-mods/litematica) (obviously the brewer is designed for Hypixel's 1.8.9 and has been thoroughly tested, I've used this brewer to brew around 1000 splashes as of feb 24). I recommend downloading litematica on the newest minecraft version (currently 1.20) and building the brewer on hypixel using this version.

*Make sure to read the tips and instructions on this page, especially the `How to use the autobrewer` section!*

If you have any other problems or questions, feel free to dm me on discord or visit my island on skyblock! discord: `bossflea` ign: `BossFlea`

## Main 35-potion bingo splashes brewer
### General features
- automatic input of awkward potions, xp boosts, spirit/mf etc.
- seperate brewer to automatically fill awkward potion storages (--> if you're having issues with the repeaters on the top not correctly updating, try adjusting the bottom repeaters like [here](https://i.imgur.com/FZfmmJN.png). This does not affect the brewer's speed)
- brew up to 192 splashes in one batch without refilling the potion ingredients
- brews (coffee etc.) have to be put into the brewing stands manually due to Hypixel's mechanics (this is unavoidable with any system)
- average time per 1 splash is *easily* under 20s from my experience (one half of a cycle takes ~20s, the other includes putting brews in, ~30s. 50s/3=<ins>16.67s</ins> per splash)

<ins>**!! Important !!**</ins> The brewer will break if you don't open every brewing stand every time before starting a brewing session! If you reload your island, this gets reset. This is another issue caused by Hypixel and is unavoidable.
Tip: Do this at the same time as you're initially filling the ingredients into the brewing stands to save time


### [XL storage variant](MainBrewer/XLstorage)
- 6 double chests of output storage per potion (373 full splashes in total)
- 'rainbow' and 'lazy' variants available
### [Large storage variant](MainBrewer/LargeStorage)
- 4 double chests of output storage per potion (255 full splashes in total)
- 'rainbow' and 'lazy' variants available
### [Medium storage variant](MainBrewer/MediumStorage) (recommended for most people)
- 3 double chests of output storage per potion (196 full splashes in total)
- 'rainbow' and 'lazy' variants available
### [Small storage variant](MainBrewer/SmallStorage) (only recommended for extremely tight chest/hopper limitations)
- 2 double chests of output storage per potion (137 full splashes in total)
- only 'lazy' variant available ('rainbow' variant not available due to space restrictions of the small size storage unit)



*More variants (especially ones with reduced potion counts) and different 'upgrade modules' in progress*

Note: Only use 'lazy' variants if you don't care about the potions not necessarily being in consistent rainbow order. *(I recently discovered that the rainbow order is largely lag dependent if you're NOT using the 'rainbow' mode, so **<ins>you'll have to try what works for you</ins>. It might just work without the slower rainbow mode for you**)* You don't lose any functionality by building the 'rainbow' variant, as you can use the rainbow variant in 'lazy' mode as well.

<details>
  <summary><ins><b><i>How to use the autobrewer</i></b></ins></summary>
  
  - First make sure you have enough xp boosts, awkward potions (let the seperate brewer run for a while, also remember to manually transfer the night vision to the main brewer's invisibility input chests), spirit/mf, wisp potions etc. in the input storage, as well as enough brews in the seperate brew dispenser.
  - Then fill your chosen amount of ingredients into the brewing stands, following the carpet color coding. Make sure to also click the brewing stands that don't need any ingredients or ones that you have already filled previously!
  - Now to start brewing, you first need to make sure the `Enable Input` lever is on. If the `Move Potions` lever is in the correct state, the brewer should start filling the brewing stands in the top row. While this is happening, manually fill the brewing stands which require brews (Do this starting from the side with the levers to avoid problems).
  - Once all brewing stands are filled, click the `Move Potions` lever. The potions will start moving down to the next layer. These ~20s are a good time to refill the agility potion's top row brewing stand with an enchanted cake from the chest above and fill your inventory with a new set of brews for the next cycle (1 brew won't fit in your inventory, use stash or ec).
  - When all the potions have finished moving down a layer, click the `Move Potions` lever again. Now repeat the two steps above until your ingredients run out.
  - To stop the awkward potions etc. from automatically being filled into the brewing stands when you want to stop brewing, set the `Enable Input` lever to off. You might also need to use this lever if the awkward potion input redstone gets stuck in the locked state while brewing.
  - Refer to [this (updated) graphic](https://i.imgur.com/7oTKKl6.png) to learn about how to retrieve splashes and in what order to splash them
    - *Make sure you don't forget any of the filler items visible in the graphic!!*
</details>

## [Alchemy 50 autobrewer](Alchemy50) (fully automatic)
### Variants
- Enchanted Fermented Spider Eye
- Enchanted Sugar Cane
### Features
- fully automatic: leave running afk and claim the xp by emptying the storage through a brewing stand
- optional glowstone functionality for some money back by npc selling
- easy to build and easily extendable (1 block wide columns)

<ins>Warning!</ins> Make sure to click every brewing stand before starting the autobrewer! Also obviously don't leave your island while the brewer is running

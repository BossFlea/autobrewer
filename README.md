# Bingo Splash Autobrewer

<!--toc:start-->

- [Bingo Splash Autobrewer](#bingo-splash-autobrewer)
  - [Feature Overview](#feature-overview)
    - [Variants](#variants)
      - [39 potions](#39-potions-download)
      - [27 potions](#27-potions-download)
  - [Building](#building)
  - [Brewing](#brewing)
    - [The `Lock Input` lever](#the-lock-input-lever)
    - [Brewing Procedure](#brewing-procedure)
      - [Preparation](#preparation)
      - [Brewing Cycle](#brewing-cycle)
      - [Finish Brewing Session](#finish-brewing-session)
  - [Splashing](#splashing)
    - [Output System](#output-system)
      - [Retrieve a Splash](#retrieve-a-splash)
      - [Remaining Splashes Counter](#remaining-splashes-counter)
    - [Splashing Order](#splashing-order)
      - [39 Potions](#39-potions)
      - [27 Potions](#27-potions)
  - [Credits](#credits)

<!--toc:end-->

This repository acts as the place to download the schematics for my Hypixel Skyblock bingo splash autobrewer and learn how to use the it! All schematics are for [Litematica](https://modrinth.com/mod/litematica).

> [!IMPORTANT]
> It is highly recommended to read all of the instructions and tips on this page, as they contain some important and useful information for building and operating the brewer!

If you have a question that isn't answered here, or you want to know something else, feel free to message me on Discord (username `bossflea`) or in-game if I'm online (ign `BossFlea`)!
You can also /visit me to see the 39-potion version.

## Feature Overview

- Automatic input of awkward potions and other base potions (XP boosts, wisp, etc.)
  - Brews (coffee, etc.) have to be inserted manually each cycle, due to Hypixel not allowing them to go through hoppers (this is unavoidable with any system)
- One-button output system: press button, take full splash out of chest
  - Optionally routes output through a brewing stand for Alchemy skill xp
- Splashes are always in rainbow order, [more information here](#splashing-order)
- Input/output storage capacity of 4 double chests (236) for each component by default (expandable)
  - Enough to brew 64 of each ingredient without interruption (192 splashes)
- Reliable redstone: zero redstone dust used, works reliably on Hypixel's broken system

### Variants

#### 39 potions [[Download Schematic](https://github.com/BossFlea/autobrewer/raw/refs/heads/main/autobrewer_39.litematic)]

- Includes all potions, even those that are broken/disabled and instant effects like Healing.

#### 27 potions [[Download Schematic](https://github.com/BossFlea/autobrewer/raw/refs/heads/main/autobrewer_27.litematic)]

- Lacks useless and broken potions that serve no purpose on bingo. **This is the recommended variant if you care about coins.**
- A good chunk cheaper than the 39-potions variant: ~30-40% cheaper per splash as of April 2026

> [!NOTE]
> The 27 potion variant makes no compromises on effects and only omits useless potions.
>
> <details>
> <summary> [expand] omitted potions </summary>
>
> - Burning (not worth the buffs)
> - Cold Resistance (useless until HotM 7)
> - Dodge (broken/disabled)
> - Fire Resistance (free from Alixer at bingo rank 0; not worth the buffs)
> - Healing (instant potion -> useless)
> - Invisibility (cosmetic)
> - Jump Boost (max level already from rabbit potion)
> - Night Vision (free from Alixer at bingo rank 0; fullbright)
> - Stamina (instant potion -> useless)
> - Stun (broken/disabled)
> - Water Breathing (not worth the buffs)
> - (Douce Pluie de Stinky Cheese (expensive))
>   - optional, can be added if desired
>
> </details>

## Building

<details>
<summary> [expand] Load and position schematic (litematica basics)</summary>

If you need more detailed instructions, there are countless tutorials for this online.

- To load a `.litematic` file, it must be in the `schematics` folder within your instance's `.minecraft` folder.
  An easy way to get there is clicking `Open Pack Folder` in the in-game options under `Resource Packs`, then navigating one level up in your file explorer. Paste the `.litematic` file in the `schematics` folder found here.
- With default keybinds, open the litematica menu using `M`, from there click `Load schematic`, where the schematic you previously copied into the folder should appear
- To position the loaded schematic, hold a stick and CTRL + Scroll until you're in the `Schematic Placement` mode. Now you can hold ALT and Scroll to move the schematic in the direction you're facing.

</details>

The schematics contain sub-regions to make it easier to build the lower parts of the brewer without your vision being obstructed by the brewing stands and other components on top.

<details>
<summary> [expand] Enable/Disable sub-regions</summary>

- Press `M` to open the litematica menu, then click on `Schematic Placements`, where you should see the autobrewer schematic. Click on `Configure`.
- In this menu, there will be a list of available sub-regions, which you can disable and re-enable using the `Placement` buttons on the right.

</details>

> [!TIP]
> I recommend starting with all the `Brewing Stands + Input XX` and `Carpets XX` sub-regions disabled in order to build the repeater layers.

Some additional tips for the building process with litematica:

- All signs will have their text automatically filled in by litematica when you place them (including color codes)
- Due to how Hypixel works, carpets can't be placed directly on brewing stands. Place them against an adjacent block instead.
- In cases where there is an item frame in the same block as a carpet, the carpet must be placed last

## Brewing

> [!WARNING]
> All brewing stands need to be opened once before you start brewing, otherwise they won't work properly on Hypixel!
> This resets when your island is unloaded (when you leave).

> [!TIP]
> Do this at the same time as inserting the brewing ingredients and modifiers for extra efficiency.

> [!WARNING]
> Note also that Hypixel sometimes takes guests' alchemy level instead of yours if they've been on your island for longer than you have, potentially ruining your potions, so be aware of that!

### The `Lock Input` lever

Clarification: This lever is simply there so you can temporarily disable the automatic input of awkward potions and other base potions in the top layer.
It is used when you're done brewing, so no new potions come in and you can finish brewing the in-progress ones in lower layers.

### Brewing Procedure

#### Preparation

- Fill the input storages with the required items (brews, xp boosts, spirit/magic find, tonic, stinky cheese)
  - The schematics include a `Shopping List` with all items required to brew a set of splashes

> [!TIP]
> For brews, use Shifty's and the Bartender's abiphone contacts if you have them unlocked (`/call shifty`, `/call bar`).
> The Crimson Isle bartenders (for Black Coffee) unfortunately don't have contacts, neither does the Melancholic Viking (Viking's Tear).
> The Fear Mongerer's contact can also be used to buy Spirit and Magic Find potions outside of an active spooky festival (`/call fear`).

> [!TIP]
> If you don't want to pay the 50k for black coffee, decent coffee from the bartender is fine as well (the stat difference is small to negligible).

<details>
<summary> [expand] Fill the water bottle storages</summary>

I recommend filling a lot of water bottles in advance, letting them go into your stash, before inserting them into their input storages.
Due to Hypixel seemingly throttling interactions with water bottles in inventories specifically, the best way to accomplish this is by dropping them:

- Use `/pickupstash` to get an inventory of bottles
- Align yourself so that the bottles will land between the two slabs in the water input areas
  - This allows both hoppers to pick them up, increasing speed
- Hold Q and quickly hover over all the bottles in your inventory to drop them
- Repeat

> [!TIP]
> Lock the 9th hotbar slot to avoid accidentally triggering the skyblock menu when holding Q.

> [!TIP]
> It can be helpful to disable your magnetic talisman to avoid picking the bottles up before they've been collected.

</details>

- Fill the brewing stands with ingredients and modifiers according to their colored carpets and item frames.
  - For the Agility potion (Enchanted Cake) fill the designated storage above instead (since they're unstackable)

> [!NOTE]
> The colored carpets indicating the ingredient types apply to the brewing stand they are placed on top of.

#### Brewing Cycle

- Make sure the `Lock Input` lever is disabled
- Press the `Advance Potions` button
- Go through all brewing stands with a dark green carpet and use the brew droppers above to dispense 3 brews to insert
  - For the Agility potion, an Enchanted Cake is dispensed along with the brews, since cakes are unstackable
- Repeat

> [!NOTE]
> If you're not using a levelled rare or higher witch pet, make sure to wait briefly (5-10s) after inserting the last brew before advancing the potions to allow it to finish brewing in time!

#### Finish Brewing Session

- When there is one ingredient left in the brewing stands of the 2nd layer from the top (green/cyan carpets), activate the `Lock Input` lever before pressing the button.
- Continue the normal cycle until all brewing stands are empty

## Splashing

### Output System

#### Retrieve a Splash

0. Make sure your inventory is completely empty
1. Press the `Request Splash` button
2. Wait briefly for the `Transfer Indicator` lamp to stop flashing
3. Take the potions out using one of two options
   a. Shift-click them out of the chest left-to-right, top-to-bottom (brewing stand disabled)
   b. Enable the brewing stand using the lever and shift-click the potions out through that to gain Alchemy XP

> [!NOTE]
> In the 39 potion variant, there will be 4 potions that don't fit into your inventory. These go into your stash:
>
> - Pick up the potion with your cursor
> - Press ESC to close the chest/brewing stand and send it to stash
> - Repeat for all 4 potions

> [!TIP]
> Set up a keybind for `/pickupstash` to use while splashing. This can be done with the Skyblocker mod using `/skyblocker shortcuts` (scroll to the bottom).

> [!NOTE]
> If you intend on using the brewing stand, make sure you don't forget the filler items in the hopper and brewing stand in the output room, as described by the signs in the schematic.

Read the [section on splashing order](#splashing-order) for more information on the rainbow order.

#### Remaining Splashes Counter

This is a simple system to indicate the number of currently stored splashes.

- After a brewing session, fill the top dropper (next to the retrieval system) with as many items as you brewed splashes (can be any stackable item).
- Whenever you collect a splash, one item will be transferred into the bottom dropper.

=> The items in the top dropper thus act as a counter of your stored splashes.

### Splashing Order

The Brewer is designed to output potions in such a way that allows splashing them in rainbow order.
Shift-click 8 potions at a time into your hotbar and splash them according to the following graphics:

#### 39 Potions

<img width="auto" height="230" alt="Image" src="https://github.com/user-attachments/assets/21505981-2f4d-4bbb-b1cd-390a9dae027f" />

#### 27 Potions

<img width="auto" height="230" alt="Image" src="https://github.com/user-attachments/assets/07349794-ac4a-4afd-8f9d-937f31c26f87" />

## Credits

The basic brewing stand arrangement is a modified version of `SCP_002`'s design.
All other systems and designs are by me (many of them iterations from my older brewers).

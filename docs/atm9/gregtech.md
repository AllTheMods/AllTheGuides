---
title: GregTech
description: 
authors: 
- Lue
- Jebraltar
---

# GregTechCEu Modern

## Overclock vs. Recipe Tier Skip

Recipe Tier Skip and Overclock are easily conflated especially since overclock cannot be triggered independently before EV. However, understanding the difference can save you time and resources!

### Recipe Tier Skip

Recipe Tier Skip refers to the ability of a multiblock to perform recipes of the next tier. For example, using LV Energy Hatches in an Electric Blast Furnace to smelt Aluminium. To trigger this, you MUST have **two** hatches of the same tier. Amperage of these hatches does not matter, you must have TWO of them.

### Overclock

For multiblocks, overclock refers to their ability to run at a higher voltage tier than their energy hatches, given enough amps. If your hatches total 4A you get one overclock, and if they total 16A you get two overclocks. Doing this before EV requires the use of two hatches (each supporting 2A), and therefore will also involve a Recipe Tier Skip. However, **using a single 4A or 16A hatch is enough to trigger one or two overclocks respectively, and *will not* trigger a Recipe Tier Skip**, as that strictly requires TWO hatches.

### Hatch Sharing

Given the conditions of overclocking, if a multiblock only has a single 2A hatch or has two 4A/16A hatches, there will be unused amps since multiblocks will not attempt to draw 2A, 8A, or 32A. If you do not want tier skip OR overclock, you can share a single 2A energy hatch between two multiblocks to give each one 1A. **Post-EV, if you want tier skip AND overclock, then share a pair of 4A/16A hatches between two multiblocks. This fulfills the "two hatch" requirement for recipe tier skip and provides 4A or 16A to each multiblock.** Note however that you should avoid sharing a pair of 2A or a single 4A/16A between multiblocks because that will not leave any unused amps for the second multiblock in the pair to run.

### Parallel

From a parallel hatch, parallel is the mechanism of doing *x* recipes at once in the same time as 1 recipe, using the voltage of *x* recipes. As parallel is more efficient than normal (imperfect) overclocking, parallel is applied to the recipe before overclocking.

### Subtick Overclock

Subtick Overclocking is the mechanism of being able to overclock a multiblock past 1 tick (0.05s) limit. It will still run at 1 tick, but the overclock is converted into a free parallel (instead of duration dividing by 2, parallel multiplies by 2). Example: Electric Blast Furnace running recipe many tiers above its base voltage.

### Perfect Subtick Overclock

The same as Subtick Overclock but instead of using imperfect OC rules (4x voltage, 0.5x duration), it uses perfect OC rules (4x voltage, 0.25x duration), which means all parallels from a Perfect Subtick Overclock are 100% efficient. Example: LCR running recipe many tiers above its base voltage.

## Autobuilding with the GT Terminal

The GregTech Terminal can help you build multiblocks automatically if you have the materials in your inventory! All you have to do is place the multiblock controller down, then crouch + right-click the controller with the terminal. However, it will make many assumptions about how to build the multiblock, so you may still need to manually move some components like hatches and busses around. 

## Added Multiblocks

ATM9 added several multiblocks for you to play with!

| Multiblock                             | Purpose                                              |
| -------------------------------------- | ---------------------------------------------------- |
| Greenhouse                             | Grows crops, just add water!                         |
| Apiary MK1                             | Produces comb blocks from bees, can harm the bees    |
| Apiary MK2                             | Produces comb blocks from perfect bees, without harm |
| Star Forge                             | Crafts the ATM Star and GregStar                     |
| Micro Universe Orb (MUO)               | Can produce power, ores, or creative items           |
| Advanced Large Chemical Reactor (ALCR) | A Large Chemical Reactor with parallel capabilities! |
| Mega Fusion Reactor                    | A Fusion Reactor with parallel capabilities!         |
| Void Miner                             | Produces ores                                        |

## Inert Nether Stars

Getting all the nether stars necessary for the ATM star is quite a process, but there's another way! ATM9 added **Inert Nether Stars** which allow you to easily turn **ONE Wither Skeleton Skull** into **SIXTEEN Nether Stars**. 

If you mix Mekanism with GT, you can get even more nether stars per wither skeleton skull!

## Blood Magic Meteors

The Mark of the Falling Tower ritual summons meteors from above full of goodies! In addition to the ones included in Blood Magic, we've added a few new ones!

### Added Meteors

| Meteor Ingredients                             | Meteor Contents                                         |
| ---------------------------------------------- | ------------------------------------------------------- |
| Intricate Hellforged Parts + 5,000,000 LP      | Demonite Ore & Reinforced Speed Runes                   |
| Unobtainium Ingot + 2,500,000 LP               | Allthemodium, Vibranium, and Unobtainium ores           |
| Naquadah Ingot + 2,500,000 LP                  | Naquadah, Plutonium, and Tungstate ores                 |
| Titanium Ingot + 1,250,000 LP                  | Sphalerite, Sulfur, and Tetrahedrite ores               |
| Arsenic Dust + 625,000 LP                      | Tantalite, Vanadium Magnetite, and Cobaltite ores       |
| 1x Compressed Diamond Block + 1,000,000 LP     | Diamond Block core and Diamond, Emerald, & Coal ores    |
| Palladium Ingot + 2,500,000 LP                 | Chromite, Bauxite, & Palladium ores                     |
| 1x Compressed Nether Star Block + 7,500,000 LP | Nether Star Blocks, Soul Sand, & Wither Skeleton Skulls |

### Bigger Meteor Variants

| Meteor Ingredients                                      | Meteor Contents                                    |
| ------------------------------------------------------- | -------------------------------------------------- |
| Samarium Iron Arsenic Oxide Block + 1,250,000 LP        | Tantalite, Vanadium Magnetite, and Cobaltite ores  |
| Indium Tin Barium Titanium Cuprate Block + 2,500,000 LP | Sphalerite, Sulfur, and Tetrahedrite ores          |
| Uranium Rhodium Dinaquadide Block + 5,000,000 LP        | Naquadah, Plutonium, and Tungstate ores            |
| Rhodium Plated Palladium Block + 5,000,000 LP           | Chromite, Bauxite, and Palladium ores              |
| Unobtainium Vibranium Alloy Block + 5,000,000 LP        | Unobtainium, Vibranium, and Allthemodium ores      |
| Wither's Compass + 9,750,000 LP                         | Demonite ore & Reinforced Speed Runes              |


> GregTechCEu Modern | [CurseForge](https://legacy.curseforge.com/minecraft/mc-mods/gregtechceu-modern/files)

---
title: A replacement startup map environment
tags:
  - mapping
  - modding
section: mapping
description: "A replacement for the default start map"
discord:
  enabled: true
  forum: tutorials
  tags:
    - blackops3
    - mapping
---
# Overview
---

![Template Map Screenshot](https://github.com/HarryBo021/Wiki/blob/main/Template%20Map/template_map_screenshot.png?raw=true)

[Replacement Template Map Download](https://github.com/HarryBo021/Wiki/blob/main/Template%20Map/hb21_template_replacement_v1.0.0.rar)

As many many will be aware, the default start map we are provided with in the Black Ops 3 mod tools has several issues that were never corrected by Treyarch. This package is a update that will overwrite those files
and provide you with an environment similar to the one we had for the WaW Mod tools. For example the default map is missing the spawners for the hell hounds, therefore will hang when they are due to spawn unless you
add or disable them.

The scope of this template is to properly set up all the things Treyarch didn't in a simple environment without adding anything to your mod tools. Then upon creating a map you have examples of how these things work
and can move/delete as you choose - or use them for reference.

The only assets added with this map are some light FX for the perk machines, no need for lighting states and editing the perk prefabs and I added the missing Widow's Wine prefab.

The only changed asset is the pack a punch prefab, which _does_ enable the lights using lightstates, as no default FX actually exists for it in any map.

---
# This includes
---

* 3 zones
* 1 example door
* 1 example debris which animates with FX
* 4 example windows with zombie spawns
* Zombie riser spawn points
* Hell hound spawners and spawn points - so the game will not just stop on reaching a dog round without being fixed anymore
* PBG Boxes
* Player respawn points for multiple zones
* 4 working mystery box locations
* Multiple wall buy weapons
* All 9 perks included and working but no machine for Electric Cherry ( with the perk change functionality enabled )
* 3 Gobblegum machines
* Lit and world fogs
* Example probes
* Example scripting for zones
* One line to change player start points at the top of the map GSC
* Pack a punch with lights
* Multiple lightstates set up
* 1 working electric trap linked to a door ( so it will not function until you open it )
* A remapped zombie spawner so it is _already_ using the correct one ( the USERMAP one )
* Other issues or unnecessary things from the default map removed or corrected
* A textured map, including caulking unseen areas for examples of good mapping practice

---
# Install
---

[Replacement Template Map Download](https://github.com/HarryBo021/Wiki/blob/main/Template%20Map/hb21_template_replacement_v1.0.0.rar)

Simply drag and drop the contents of the download in to your Black Ops 3 root directory and say _yes_ to overwriting the files.

Thats it! When creating a new zombie map as normal, you will now be greeted with the updated start up environment!

---
# Notes
---

You may noticed that the Gobblegum machine has missing textures, and no model shows on Deadshot Daquiri's prefab. These will both function correctly in game however. The assets were not included in the mod tools by Treyarch but _are_ loaded in the game.

If you would like to correct these in radiant, downloading Midgets T7 Asset pack will add all the missing assets and far more

[Midget Blasters T7 Asset Pack](https://github.com/MidgetBlast/T7-Assets)

---
# Credits
---
Harry Bo21

KingslayerKyle

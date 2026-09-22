---
title: Increasing the weapon table limit for mystery box guns
tags:
  - scrtiping
  - weapons
  - mystery box
section: scripting
description: "Use multiple weapon tables to get around the weapon table limit"
discord:
  enabled: true
  forum: tutorials
  tags:
    - blackops3
    - mapping
---
# Overview
---

The mystery box and wall weapons rely on weapon tables in order to work. These contain settings such as prices and if the weapons should appear in the mystery box. However these tables have a limit ( I think its 48 
but I cannot remember exactly ).

This can pose a problem if you want a lot of weapons in your map, you may have guns showing as costing 0 points, or simply never showing showing in the box rotation.

Dont worry, there is a very simple solution.

You can use more than one weapon table, the game will respect this. I have done this often to add additional weapons to stock maps, without making any changes to the original table.

---
# The weapon tables
---

Weapon tables are located in `share\raw\gamedata\weapons\zm`

Create your new table here, and add any guns you want. Im not sure how this will work if a gun exists in more than one table. One entry will definitely take priority over the other, but which is anyones guess.

In `your map name.zone` you will need to add the table like so :

```cpp
stringtable,gamedata/weapons/zm/zm_my_table.csv
```

---
# Scripting
---

This is really simple, in *BOTH* your `mapname GSC and CSC` find and locate this code :

```cpp
function custom_add_weapons()
{
	zm_weapons::load_weapon_spec_from_table("gamedata/weapons/zm/zm_levelcommon_weapons.csv", 1);
}
```

All you need to do, is duplicate the line and rename it to yours :

```cpp
function custom_add_weapons()
{
	zm_weapons::load_weapon_spec_from_table("gamedata/weapons/zm/zm_levelcommon_weapons.csv", 1);
	zm_weapons::load_weapon_spec_from_table("gamedata/weapons/zm/zm_my_table.csv", 1);
}
```

Thats it! The game will now properly load both tables side by side, breaking the arbitrary limit, or allowing you to simply add to a maps existing table without changing it.

---
# Credits
---
Harry Bo21

KingslayerKyle

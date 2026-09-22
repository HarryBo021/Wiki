---
title: Splitting large zones
tags:
  - mapping
  - zones
  - zombie spawning
  - player respawning
section: mapping
description: "Isolated zones, areas you may warp to and from that you do not want zombies spawning in if there are no players in them"
discord:
  enabled: true
  forum: tutorials
  tags:
    - blackops3
    - mapping
---
# Overview
---

There may be times you have a zone away from the action, that perhaps players will teleport to and away from. Or perhaps a area you can drop down from, but not get back up to the same way. These are zones
we do *NOT* want to treat as adjacent zones. 

We only want zombies to be spawning in these areas, when someone is actually inside them.

This is actually very simple.

---
# Scripting
---

Open `your map name.gsc` and find this

```cpp
init_zones[0] = "start_zone";
```

Simply add your zone to the list like so :

```cpp
init_zones[0] = "start_zone";
init_zones[1] = "teleport_zone";
```

This zone will now only act as active, when someone is actually in it.

---
# Credits
---
Harry Bo21

KingslayerKyle

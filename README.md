# Tapchanger lite

A lightweight toolchanger for Voron 2. A rewrite from [Tapchanger](https://github.com/viesturz/tapchanger) that is easier to build and run but not as rigid. Primarily aiming to support Mini Stealthburner and other lightweight toolheads.

The cool stuff over regular Tapchanger:

- lightweight, the shuttle + mounting plate is only 42g, half of normal Tap weight
- self locating and tolerant to ~1mm offsets on all axis.
- zero Z travel on the hotend when docking, allowing to install wipe pads, etc
- 3x faster dock sequence with only 16mm z travel, still need to move up to the tool parking area though
- no moving parts, except the bearings
- significantly cheaper to make, because no rail needed

The questionable stuff:

- def less rigid than the linear rail

![Preview](/Images/hotend-shuttle.jpg)

# How does this work?

It's essentially an oversized linear rail, that supports only ~4 mm of travel.
The steel rail is replaced by small rail fragments where actual contact takes place.
The bearings take place of the balls, and we can get away with only 3 per side.

In addition it's a kinematic mount, meaning that it's self aligning and there is no play even if the parts are not aligned precisely.
The two middle bearings ride on socket scew heads providing a somewhat flat surface and adjustability to tension the mount.

![Preview](/Images/explain1.png)
![Preview](/Images/explain2.png)


# Community

Improvement ideas - bugs, pull requests welcome. Or find me on [Voron Toolvchangers Discord](https://discord.gg/KfdJ25vk), or file bugs here.

See Tapchanger [youtube channel](https://www.youtube.com/playlist?list=PLqU7kX5nUJDRDw5z0NLwJ22OkV6fbjnSW).

# Build guide

Check the [bom](./Bom.md).

Start with [Printing](./Print%20Guide.md)

Assembly instructions coming...

Firmware - see [Tapchanger repo](https://github.com/viesturz/tapchanger/tree/main/klipper).

# Credits

- Basic models from [Voron Stealthburner](https://github.com/VoronDesign/Voron-Stealthburner) and [Voron 0](https://github.com/VoronDesign/Voron-0).
- Mini SB Orbiter cowling form [mozartlovescats](https://www.printables.com/model/366337-voron-02-orbiter-20-trianglelab-chc-mini-stealthbu).
- Mini SB LGX lite cowling form [MC](https://www.printables.com/model/395933-voron-02-mini-stealthburner-remix-for-lgx-light-ex/files).

# Revision history:

## V1.1 - Verified and cleaned up.

- Minor model tweaks for better fit and printability.


## V1 - This should work

- Redesigned and optimized - not compatible with V0
- Significanly more rigid
- Supports both Mini and full size Stealthburner

## V0 - Initial drop
 
 - It can print and looks reasonably rigid
 - ~10 Tool chnages so far
 - Initial dock, that looks okay for the job

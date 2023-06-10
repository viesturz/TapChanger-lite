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
- shuttle heatset inserts require accurate angle to get right.

![Preview](/Images/plate.jpg)
![Preview](/Images/shuttle.jpg)
![Preview](/Images/dock.jpg)

# How does this work?

It's essentially an oversized linear rail, that supports only ~4 mm of travel.
The steel rail is replaced by small rail fragments where actual contact takes place.
The bearings take place of the balls, and we can get away with only 3 per side.

In addition it's a kinematic mount, meaning that it's self aligning and there is no play even if the parts are not aligned precisely.
The two middle bearings ride on socket scew heads providing a somewhat flat surface and adjustability to tension the mount.

![Preview](/Images/explain1.png)
![Preview](/Images/explain2.png)



# Building

This is **work in progress**, you will need to borrow a lot of stuff from the [Tapchanger](https://github.com/viesturz/) repo.

# BOM

All standard Voron stuff.

**Shuttle:**
 
 - X6 [F623-RS](https://google.com/search?q=F623-RS) Bearings, flanges are optional. Same as regular Voron BOM.
 - X6 M3x8 buttonhead screws, m3 washers and heatset inserts.
 - 6x3mm round magnet

**Toolhead mounting plate:**

 - Tap optical sensor
 - 2x m3x4 buttonhead screws to secure the sensor
 - 2x m3x6 SHCS screws
 - 4x steel pads - 10x4mm 1.5mm thick, im cutting them from a stock piece from local hw store
 - some glue to hold the pads in place


 **Dock:**

 - 3x heatset inserts
 - 2x m3x6, 1x m3x8
 - Some silicone for the nozzle pad
 - a small piece of spring to hold up the nozzle pad
 - 2x 5x2 round magnets - attached to the miniSB crew heads

# Revision history:

## V0 - Initial drop
 
 - It can print and looks reasonably rigid
 - ~10 Tool chnages so far
 - Initial dock, that looks okay for the job

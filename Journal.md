# [Kratos] - Personal Log

## Section 1: My History with 3D Printers
My first 3d printer similar to many in the 3d printing community was an ender 3. Being now an 8 year old printer, it had many issues, from the very primitive POM wheels causing a multitude of problems, and the tedious manual bed leveling. These struggles led me down a rabbit hole of upgrading and modifying my printers, I first added a second lead screw to convert it to dual Z axis, to reduce z wobble and to handle the weight of a direct drive extruder mod. And I even ended up adding new bigtreetech board. For the past 4 years I have modded upgraded and fixed any printer I could get my hands on anywhere from an ender 3 v2 neo, to a ankermake m5c, and even recently a bambu lab a1 mini. Eventually I had had enough with the low build/print quality, or the closed off an proprietary hardware and software, on commercial machines, so I decided to build Kratos, compiling all the skills I have learned over the past several years

## Section 2: Kinematic & Architectural Choices
* **CoreXY vs. Bed Slinger:** I decided a coreXY build would be more fitting for Kratos then a bed slinger, or a flying bed coreXY for a few specific reasons. Bed slingers found on budget 3d printers are known to have many issues such as, the vibrations and shaking produced by the extruder head printing at higher speed often cause z wobble meaning gantry holding the extruder shaking so the layer have ringing or other artifacts. In addition moving the have heavy bed side to side having to immediately flip the direction when printing is a severe issue limiting print speed and quality. A coreXY design solves these issues by having the bed move up and down limiting the amount of fast back and forth movements it has to do, aswell as limiting the weight to move the extruder head meaning overall faster print speed. A flying bed printer has a very similar problem to a bedslinger but instead of having to move a heavy bed side to side they are moving the whole x and y gantry up and down meaning you are now carrying the weight of linear rails, aluminum extrusions, motors ect and you have to deal with keeping it perfectly paralel to the bed. ALl of these drawbacks led me to make the most important decision for this printer of making it a coreXY design.
* **Motor Placement:** [Describe your CAD iterations for motor layout...]

## Section 3 XY gantry
I am going to talk about my dfirst ideas for the frame in the archive and then why i decided to scrap that and do a reset and restart my corner mounts and all the other big mounting decisions i made

## Section 4 Kinematic bed/Triple Z axis system

## Section 5 Software Klipper vs Marlin

## Section 6: Component Decisions
### Toolhead Choice
[Write about why you picked Stealthburner, the Bambu hotend, and printing the body...]

### Why I chose a voron bed kit

### Power & Electronics
[Write about the Octopus Pro board, BTT CB1, and the AC bed wiring...]

## Calibration and Setup

## Section 7 Future of Kratos

# [Kratos] - Personal Log

## Section 1: My History with 3D Printers
My first 3d printer similar to many in the 3d printing community was an ender 3. Being now an 8 year old printer, it had many issues, from the very primitive POM wheels causing a multitude of problems, and the tedious manual bed leveling. These struggles led me down a rabbit hole of upgrading and modifying my printers, I first added a second lead screw to convert it to dual Z axis, to reduce z wobble and to handle the weight of a direct drive extruder mod. And I even ended up adding new bigtreetech board. For the past 4 years I have modded upgraded and fixed any printer I could get my hands on anywhere from an ender 3 v2 neo, to a ankermake m5c, and even recently a bambu lab a1 mini. Eventually I had had enough with the low build/print quality, or the closed off an proprietary hardware and software, on commercial machines, so I decided to build Kratos, compiling all the skills I have learned over the past several years

## Section 2: Kinematic & Architectural Choices
* **CoreXY vs. Bed Slinger:** I decided a coreXY build would be more fitting for Kratos then a bed slinger, or a flying bed coreXY for a few specific reasons. Bed slingers found on budget 3d printers are known to have many issues such as, the vibrations and shaking produced by the extruder head printing at higher speed often cause z wobble meaning gantry holding the extruder shaking so the layer have ringing or other artifacts. In addition moving the have heavy bed side to side having to immediately flip the direction when printing is a severe issue limiting print speed and quality. A coreXY design solves these issues by having the bed move up and down limiting the amount of fast back and forth movements it has to do, aswell as limiting the weight to move the extruder head meaning overall faster print speed. A flying bed printer has a very similar problem to a bedslinger but instead of having to move a heavy bed side to side they are moving the whole x and y gantry up and down meaning you are now carrying the weight of linear rails, aluminum extrusions, motors ect and you have to deal with keeping it perfectly paralel to the bed. ALl of these drawbacks led me to make the most important decision for this printer of making it a coreXY design.
* **Frame and structural integrity:** A 3d printer has to deal with many forces whether those be linear, horizontal, rotational, or even the vibrations of all of the moving pieces moving and forth at such a rapid rate. But this means that the frame of a 3d printer needs to be a ble to handle all of these forces and make sure to keep as little stress on other less structural pieces. My thinking when I think of something that needs to be very strong and structural I think of screws. Screws are one of the first things you grab for when you have to make something strong, but trying to use screws to hold these aluminum extrusions proved to be a lot more difficult than I first thought. My initial idea was to screw them in from the corners but this led to a problem, I had to hold 3 pieces In a corner all facing different directions meaning I had to use a minimum of two screws, but no matter how I tried I couldnt get two screws in without them intrfering with eachother. To my misfortune that wasnt even the hardest part of trying to use screws, I would have to tap the screw and do it straight on and make sure to keep it perfectly straight. In addition when I would be assembling it I would have to use a machinists square to ensure that the frame was totally square, and if it wasn't I would have to drill another hole into the metal. Everytime I drilled into it again it compromised the structural Integrity of it further. Eventually I decided I could make a 3d printer piece to keep the metal firmly together, it would be adjustable so If I wanted to change the design or a piece broke I could just unscrew it print another one and I'd be back up and running. So for the last several months I have been working through many iterations to get the best design that would meet all of my criteria. <p align="center">
  <img src="pictures/Old%20parts%20picture.jpg" alt="Graveyard of early iterations" width="250px" />
  <br />
  <em>Figure 3.1: Graveyard of early iterations, test mounts, and discarded CAD prototypes.</em>
</p>

## Section 3 XY gantry
I am going to talk about my dfirst ideas for the frame in the archive and then why i decided to scrap that and do a reset and restart my corner mounts and all the other big mounting decisions i made
* **Motor Placement:** My first instinct regarding the motor placement was to place it on the inside of the of the extrusions, this can be seen in side my archive Kratos build. This was my first big mistake, as this made me spent many weeks frustrated on how to do the belt routing. But I was way overcomplicating it, because having the motor on the inside of the corner made the printer not be aligned with the linear rails which is crucial for belt tensioning, as if it isnt perfect straight when the y axis moves it would change the tension of the belt. After many hours spent trying to figure out the belt routing I went back to look at other coreXY designs to see waht they did, and to get inspiration from it. After just minutes of googling I realized I had to scrap everything I had just spent so much time fixing. I had built my corner pieces around the motor on the inside of the build and after looking at other printers such as the voron trident, I saw they placed motor along side the outer edges of the frame allowing it to be perfectly aligned with the linear rail and with the next corner it had to go to. This meant simplyifying my design that at one point had four idlers at each corner down to only two at two of the corners.
| Original Design (Internal Motor) | Redesigned Mount (Outer Motor) |
| :---: | :---: |
| <img src="pictures/Old%20corner%20mount.jpg" width="250" /> | <img src="pictures/New%20corner%20mount.jpg" width="250" /> |

*Figure 3.2: Comparison between the original internal motor design with complex belt routing (left) and the updated outer-mount design (right).*
*Figure 3.2: Comparison between the original internal motor design with complex belt routing (left) and the updated outer-mount design (right).*
*Figure 3.2: Comparison between the original internal motor design with complex belt routing (top) and the updated outer-mount design (bottom).*
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

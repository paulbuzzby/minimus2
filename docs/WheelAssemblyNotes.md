
# Wheel Assembly

The wheel assembly is a surprisingly difficult part to design. This part needs to hold the motor and wheel system along with the encoder. All of this needs to be in a compact and small space.
The overall width of the system is dictated by the choice of motor as the motors will effectively be end to end. 

An asymmetric design is not possible on this mouse. This means that the wheel assembly will be mirrored from left to right sides.  

A critical decision is the gear ratio and the gears. The spec of the gears fixes the size of the gears and the centre to centre distance. This has a knock on effect of, somewhat, fixing the wheel and tire size.

Other critical choices include bearing sizes and attachment hardware sizes.
As an example of some of the difficulties. A standard M2 bolt has a head that is 2.5mm thick. If such a bolt is used to attach the wheel this is 5 mm of space taken up across the width of the mouse with bolt heads.
The mouse is **only** 38mm wide. 

Another critical choice is how this wheel assembly is mounted to the PCB chassis of the mouse. Any holes and mounting area used on the PCB represents PCB area that cannot be used to mount components.

The choice of encoder must be decided before the assembly can be designed as this must be integrated into the design.
A magnetic encoder has been chosen. The exact model is now less critical but we now know that a magnet must be mounted and rotated along with the wheel.

To get started with this design process some restrictions must be set.

# Goals
 

 - Easy of manufacture
	 - No special materials
	 - Hobby based equipment
	 - Ideally all components can be bought off the shelf. We would like to avoid the custom manufacture of as many items as possible.
	 - The used of hobby grade FDM and / or resin 3D printing is expected
 - As compact as possible
 - Repeatable

# Component choice / restrictions

The following choices have been made that help to constrain the system

- M2 hardware
- 0612 DC coreless motors
- 5:1 gear ratio made up of a 40T spur and 8T pinion
	- 40T has a 2mm ID
	- 8T pinion has a 0.75mm ID for push fit onto the 0612 motors
	- Gears are **NOT** to be 3D printed
- MF52zz bearings
- Need at least 1mm gap between bottom of chassis and maze surface
- Around a 14mm tire
	- The wheel will be designed to work with the final choice of tire.
	- 


# Sources for components


- Gears
	- 40T gear https://www.aliexpress.com/item/1005005234726449.html
		- 1.5mm thick, these also come with 8T pinions
	- Pinions https://www.aliexpress.com/item/1005004099237598.html
- Motors
	- 0612 DC coreless https://www.aliexpress.com/item/1005007681813603.htm
- M2 Hardware
	- Lots of sources but in UK https://www.ebay.co.uk/str/kaysfasteners for most
	- Thin head M2 https://www.ebay.co.uk/itm/326445351215
- Radial / diametrically opposed magnets
	- AlieExpress https://www.aliexpress.com/item/1005009202333053.html
	- UK https://magnetstore.co.uk/disc-magnets/6mm-x-3mm-disc-diametrically-magnetised-neodymium-n52-0-31kg-pull/
- Bearings (MF52zz)
	- Amazon (UK) https://amzn.eu/d/jhKqFhr
# Swadge SAO

These are [Simple Add-ons (SAO)](https://hackaday.io/project/52950-shitty-add-ons/log/159806-introducing-the-shitty-add-on-v169bis-standard) of Swadges ([MAGFest's](https://www.magfest.org/) swag badges). They are meant to decorate full size Swadges, but can be used on any badge with a SAO connector.

These [KiCad](https://www.kicad.org/) projects can be manufactured and assembled by [JLCPCB](https://jlcpcb.com/), though any PCB manufacturer should be capable. The parts used already have [LCSC](https://www.lcsc.com/) numbers and the projects can be easily exported using [Fabrication ToolKit](https://github.com/bennymeg/JLC-Plugin-for-KiCad). The projects are designed to be fabricated using [JLCPCB's "Economic PCB Assembly"](https://jlcpcb.com/capabilities/pcb-assembly-capabilities), which means:
* Two layers
* Board size between 10x10mm - 570x470mm
* 0402 minimum package size
* Single sided part placement (SMT/Thru-hole)
* No Gold Fingers, castellated Holes, or edge Plating
* Order in QTY 30 or 50, depending on color

It is also recommended to manually [add tooling holes](https://jlcpcb.com/help/article/47-How-to-add-tooling-holes-for-PCB-assembly-order). If you don't, then JLCPCB's engineers will add the holes themselves and validate their placement with you before manufacturing. The requirements are:

1. Two or three tooling holes should be added on the PCB, they should be placed in opposite corners of the PCB and as far apart from one another as practical.
1. Tooling holes should be 1.152mm(45.4mil) round non-plated holes with 0.148mm solder mask expansion.
    > A `tooling_hole` footprint is provided in the `sao` footprint library.
1. Tooling holes are only required for PCB assembly orders.
1. Please try to add tooling holes on empty space and keep them away from traces. If there is no enough room, you can add them to the copper area.

## squarewavebird_sao

This is a SAO of the Squarewavebird Swadge. The source Swadge can be found at https://github.com/AEFeinstein/Super-2023-Swadge-HW.
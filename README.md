# Num64
![Num64_Logo](https://github.com/user-attachments/assets/c10de669-2bbc-4003-90f6-a164e7adf4be)

3D printer files and Gerber files

STL files were printed on SOVOL SV06+ with a 300mmx300mmx340mm bed size. 

## Printer settings:
- .6mm nozzle
- layer height: .4mm
- first layer: .3mm
- infill: 20%

hardware required:
- Nice!nano v2 controller
- M3x3x5 heat sink threaded insets
- M3x8 hex bolts
- [Battery](https://a.co/d/9JyL29i)
- *Optional* [JST 1.25mm 2 Pin connectors](https://a.co/d/bhRtTt9)

## Build Steps

1. Print the plate
2. Solder diodes to PCB
3. Solder RGB LED to PCB *config not working at this time*
4. *optional* Solder JST connector to controller
5. Solder controller to PCB
6. Flash the controller with [firmware](https://github.com/Glitch860/zmk-config-num64)
   - Under the master branch select Actions
   - Choose the latest successful workflow
   - Under the workflow artifacts download the firmware file
7. Using a soldering Iron heat sink the threaded inserts into the plate on the front and back
8. Pop switches into the plate *60 in total needed*
9. Align the plate with switches onto the PCB
10. Solder all 60 switches to the PCB
11. Print the back and front pieces
12. Place the battery in the back base cutout
13. connect the battery using the JST connector. OR solder directly to the controller
14. Using the M3x8 bolts screw the front and back to the plate

# License

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1"></a></p>

You are free to:

Share — copy and redistribute the material in any medium or format

Adapt — remix, transform, and build upon the material

The licensor cannot revoke these freedoms as long as you follow the license terms.
Under the following terms:

Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

NonCommercial — You may not use the material for commercial purposes.

ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

No additional restrictions — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

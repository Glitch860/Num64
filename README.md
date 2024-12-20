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
- *Optional* SMB power switch or [Battery helper](https://www.boardsource.xyz/products/Battery-Helper)

## Build Steps

1. [Print the plate](https://github.com/Glitch860/Num64/blob/main/NUM64_plate.stl)
2. While the plate is printing. Dend 60 diodes:

![PXL_20240911_173447660](https://github.com/user-attachments/assets/980fea1f-aa7f-4726-8849-31ba3a4a1f1c)

3. Solder diodes to PCB by putting them through the holes on the back side of the PCB. Bend the legs to help hold it in place. Make sure the black line of the diode is matching the silkscreen.

![PXL_20240911_173520431](https://github.com/user-attachments/assets/396bf678-e249-4caa-93b7-3801f9708c5f)

4. Clip the diode legs once they a soldered.
   >Be sure to save the diode legs for a later step.
  
5. Solder RGB LED to PCB *config not working at this time* The cruved pin is ground. Solder LED's as shown

![PXL_20240911_173824425 MP~2](https://github.com/user-attachments/assets/23e622ce-597d-48ed-b715-f72add3d1110)
   
6. *optional* Solder JST connector to controller. Red wire solder to + and black wire to - 
7. Solder hot swap controller sockets to the PDB
8. Using the diode legs mount the controller in the hotswap sockets. Solder and clip the legs.
9. Flash the controller with [firmware](https://github.com/Glitch860/zmk-config-num64)
   - Under the master branch select Actions
   - Choose the latest successful workflow
   - Under the workflow artifacts download the firmware file
10. To flash the firmware use a pair of twizzers and touch the Gnd and Rst pins on the controller. You should see a drive call *NICENANO* show up.
    - Drag and drop the .uf2 file onto the mounted NiceNano drive
    - After a successful copy the drive will unmount and your keyboard should be working
    - *recommend* testing the PCB with an online keyboard tester. Using a pair of twizzers touch both holes of each switch.
11. Pop switches into the plate *60 in total needed*, be sure to firmly push the switch into each hole.
12. Align the plate with switches onto the PCB. Be sure no not to bend any of the switch legs. You will have to push the PCB and plate together to ensure the switch *CLICK* into place.

![PXL_20240911_200120786](https://github.com/user-attachments/assets/3972fcc5-d4da-48dd-915a-293151151fb9)
   
13. Solder all 60 switches to the PCB

![PXL_20240911_200334668](https://github.com/user-attachments/assets/af46c8ae-d17c-41e7-b5e1-54b6190abc4f)

14. Strip a small piece of wire and solder it to D59. Connecting the two switches at the bottom.
   >This was a step missed in the design process. This should be corrected in newer releases on this Repo.

![PXL_20240911_193548092](https://github.com/user-attachments/assets/c8f28440-cd71-4596-b944-d5c0aa268091)

15. Print the [back](https://github.com/Glitch860/Num64/blob/main/Num64_Back.stl) and [front](https://github.com/Glitch860/Num64/blob/main/Num64_Front.stl) pieces
16. Place the battery in the cutout on the back piece.
17. connect the battery using the JST connector. OR solder directly to the controller
18. Using the M3x8 bolts screw the front and back to the plate
19. Put some little rubber feet on the bottom of the front and back pieces.
20. Enjoy your new keyboard.

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

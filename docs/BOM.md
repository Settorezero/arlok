## ARLOK Bill Of Materials

### Summary

1) Electronics - PCB
2) Electronics - Shield Components
3) Electronics - External components
4) Mechanics   - 3D-printed parts
5) Mechanics   - Components

### 1) Electronics - PCB

Step 1: Subscribe to PCBWay using my invite link:
        https://www.tinyurl.com/pcbwaysz

Step 2: Order the ARLOK shield PCB from the following link:
        https://tinyurl.com/arlokshield

### 2) Electronics - Shield Components

| Part         | Value                                          | Notes                            |
|--------------|------------------------------------------------|----------------------------------|
| C1           | 100nF multilayer                               | pitch 5mm                        |
| C2           | 100nF multilayer                               | pitch 5mm                        |
| C3           | 1000uF 16V electrolytic                        | pitch 3,5mm dia 8mm              |
| C4           | 100nF multilayer                               | pitch 5mm                        |
| C5           | 100nF multilayer                               | pitch 5mm                        |
| C6           | 100nF multilayer                               | pitch 5mm                        |
| D1           | 1N400x  (good 1N4001, 1N4007 ecc)              |                                  |
| R1           | 22K ¼W                                         |                                  |
| R2           | 15K ¼W                                         |                                  |
| R3           | 330 ¼W                                         |                                  |
| P1           | tactile switch 6x6mm (long button)             |                                  |
| P2           | tactile switch 6x6mm (long button)             |                                  |
| RESET        | tactile switch 6x6mm                           |                                  |
| VR1          | Trimmer 10K                                    | Type PT10LV10                    |
| L1           | led 3mm                                        |                                  |
| H1           | male pinheader 10pin                           | Arduino header - solder on top   |
| H2           | male pinheader 8pin                            | Arduino header - solder on top   |
| H3           | male pinheader 5pin                            | Arduino header - solder on top   |
| H4           | male pinheader 4pin                            | Arduino header - solder on top   |
| EXT (EXT1)   | male pinheader 7pin                            |                                  |
| EXT2 (A1)    | male pinheader 3pin                            |                                  |
| EXT3 (A2)    | male pinheader 3pin                            |                                  |
| EXT4 (A3)    | male pinheader 3pin                            |                                  |
| HC-SR04      | male pinheader 4pin                            |                                  |
| I2C          | male pinheader 4pin (optional)                 |                                  |
| J1 (COMM)    | female pinheader 6pin                          |                                  |
| JP1          | male pinheader 3pin + jumper                   |                                  |
| JSW(POWER)   | male pinheader 2pin + jumper OR 2.54mm switch  |                                  |
| LEFT_SERVO   | male pinheader 3pin                            |                                  |
| RIGHT_SERVO  | male pinheader 3pin                            |                                  |
| OLED         | female pinheader 4pin                          |                                  |
| X1           | Screw Terminal 2pin                            | Pitch 5mm                        |
| X2           | Screw Terminal 2pin                            | Pitch 5mm                        |
| GROVE        | GROVE male header (optional)                   |                                  |

### 3) Electronics - External components

| Qt.          | Description                                      |
|--------------|--------------------------------------------------|
| 1x           | MakerUNO board by Cytron                         |
| 2x           | Servo MG996R modded for continuos rotation       |
| 1x           | HC-SR04 Ultrasonic sensor                        |
| 1x           | Bluetooth module HC-05 or HC-06                  |
| 1x           | OLED display module I2C (4pin) 0.96"             |
| 1x           | Battery Holder for 4AA batteries                 |
| 1x           | Battery Holder for 3AA batteries                 |
| 1x           | Round pushbutton with retain or lever switch (*) |
| 7x           | AA 1.5V Batteries (**)                           |

(*)  Print the "arlok_pillar_hole_xx.stl" according the pushbutton diameter  
(**) Not adviced to use NiCd or NiMH batteries, since voltage of those batteries is 1.2V. 
     Eventually you can use only 4NiMH batteries in the 4AA battery holder and don't use the 
     3AA battery holder: then you can power all robot using the 4AA. In this case don't mount
     D1 (put a piece of wire and pay attention to power orientation), put the power jumper JP1
     in VSERVO position and keep the fingers crossed: the servo will absorb more current and
     malfunction (such as resets on board or on the bluetooh module) can occur. This solution
     is NOT tested!

### 4) Mechanics - 3D-printed parts

Please see in the [STL folder](../stl)

### 5) Mechanics - Components

| Qt.          | Description                                                                  |
|--------------|------------------------------------------------------------------------------|
| 12x          | M3 screw, Allen bolt socket cap, 12mm (length of threaded part - 15mm total) |
| 8x           | M3 screw, Allen bolt socket cap, 5mm (length of threaded part - 8mm total)   |
| 14x          | M3 washers (optional)                                                        |
| 14x          | M3 nuts                                                                      |
| 2x           | M3 screw, Countersunk, 8mm (length of threaded part, 10mm total)             |
| 4x           | Hex Standoff 10mm                                                            |
| 1x           | Tamiya BallCaster model 70144                                                |
| 2x           | Rubber O-Ring, 70mm internal diameter, 2-3mm width                           |
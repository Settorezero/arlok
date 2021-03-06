## Connections
In the following table are showed Arduino Uno/MakerUNO to Arlok shield connections.  

> Pinout is reported also for the older version named AR.L.O.  

If a cell is empty, means that pin is free to use and reported on a dedicate header. The `interrupt` column shows the interrupt number associated with the pin (valid only for boards with the ATmega328), but is reccomended to use the Arduino function `digitalPinToInterrupt(Pin)` such as used in the Arlok sketches.

| Arduino PIN | AR.L.O. (obsolete)    | Arlok (current)                           | Notes                    | Interrupt |
|:------------|:----------------------|:------------------------------------------|:-------------------------|:----------|
| (empty)     |                       | Not available                             | The unused pin near IOref|           |
| IORef       |                       | Not available                             |                          |           |
| Reset       | Reset Button          | Reset Button                              |                          |           |
| 3.3V        |                       |                                           |                          |           |
| 5V          |                       |                                           |                          |           |
| GND         |                       |                                           |                          |           |
| GND         |                       |                                           |                          |           |
| Vin         |                       | Not available                             | unused on MakerUNO       |           |
| A0          | Trimmer VR1           | Trimmer VR1                               |                          |           |
| A1          |                       |                                           |                          |           |
| A2          |                       |                                           |                          |           |
| A3          |                       |                                           |                          |           |
| A4          | Don't use if OLED!    | Not available                             | Shared with SDA          |           |
| A5          | Don't use if OLED!    | Not available                             | Shared with SCL          |           |
| D0/RX       | UART RX > COMM RX     | UART RX > COMM RX                         |                          |           |
| D1/TX       | UART TX > COMM TX     | UART TX > COMM TX                         | Through voltage divider  |           |
| D2          | Sonar - Echo          | Pushbutton 1                              | 'button' on MakerUNO     | 0         |
| D3          |                       | Sonar - Echo                              |                          | 1         |
| D4          |                       | Sonar - Trigger                           |                          |           |
| D5          |                       | Pushbutton 2                              |                          |           |
| D6          | Pushbutton 1          |                                           |                          |           |
| D7          | Pushbutton 2          |                                           |                          |           |
| D8          | Sonar - Trigger       | Buzzer (if makerUNO is used)              | 'buzzer' on MakerUNO     |           |
| D9          | ServoMotor - Right    | ServoMotor - Right                        |                          |           |
| D10         | ServoMotor - Left     | ServoMotor - Left                         |                          |           |
| D11         |                       |                                           |                          |           |
| D12         |                       |                                           |                          |           |
| D13         |                       |                                           |                          |           |
| GND         |                       |                                           |                          |           |
| ARef        |                       |                                           |                          |           |
| SDA         | OLED SDA              | OLED SDA + Grove + I2C header             | Shared with A4           |           |
| SCL         | OLED SCL              | OLED SCL + Grove + I2C header             | Shared with A5           |           |

### Connections considerations
- On Arlok shield some pin are not reported on the PCB (such as the `IOref` and the unused pin near it, `A4` and `A5`), so you can use fewer male headers.
- On both Arlok and AR.L.O., `A3` is used in some sketches as seed for random number generator initialization; so, if you want to use `A3` in your own application, please change the code accordly.
- On Arlok all free digital pins are reported on `EXT` header along with 5V and ground, and the 3 free analog inputs are reported on 3 separate headers having power supply each while on on AR.L.O. free digital pins are reported on 2 headers: `EXT2` (`D11`, `D12`, `D13`) and `EXT1` (`D3`, `D4`, `D5`) and the analog inputs are reported to simple pads.

# FB-32G CD32 Riser Gamer Module

This is first module created for the FB-32R CD32 Riser
It has the following features:

Amiga 23pin Scart Video Connector (non-Genlock)
Minimig Scart output (with Ian Stedmans 3.3V Sync level correction which is selectable via jumper JP1)
Audio Jack
PS/2 Keyboard Interface - using the PIC16F628A (in a SSOP Package) running the same code as Kipper2K's CD32 riser
RS232 Serial - Basic Non-handshaking

# Build Notes:
Solder the PIC Microcontroller first and program it before adding any other componenets due to pin 4 being being used as part of the keyboard implementation and causes issues with programming once the board is built...you have been warned!

## License

This project and all the files contained are released under the GNU GPLv2. If you build a modified version of the board you must supply the end user with all the sources (this can be a web link).

# Bill of Materials

|Part | Value | Device | Package | Description |
|-----|-------|--------|---------|-------------|
| IC1  |       |SN74LVC1G97| SOT-23-6 | Configurable Gate |
| IC2  |       |SN74LVC1G97| SOT-23-6 | Configurable Gate |
| IC3  |       |SRV05-4| SOT-23-6 | Diode Array           |
| IC4  |       |PIC16F628A|SSOP-20| Microcontroller       |
| IC5  |       |MAX3311|uMAX-10| RS-232 Tranceiver        |
| U1   |       |LM1117-3.3| SOT-223 | Voltage Regulator   |
| C1   | 10uF  |Capacitor| 1206 | Ceramic                 |
| C2   | 10uF  |Capacitor| 1206 | Ceramic                 |
| C3   | 100nF |Capacitor| 0603 | Ceramic                 |
| C4   | 100nF |Capacitor| 3x5.3mm | Electrolytic         |
| C5   | 100nF |Capacitor| 3x5.3mm | Electrolytic         |
| C6   | 100nF |Capacitor| 0603 | Ceramic                 |
| C7   | 6800pF|Capacitor| 0603 | Ceramic                 |
| C8   | 6800pF|Capacitor| 0603 | Ceramic                 |
| C9   | 100nF |Capacitor| 0603 | Ceramic                 |
| C10  | 100nF |Capacitor| 0603 | Ceramic                 |
| D7   |       |1N914| SOD-323 | Diode                    |
| R1   | 75R   |Resistor| 0603 |                          |
| R2   | 75R   |Resistor| 0603 |                          |
| R3   | 1K    |Resistor| 0603 |                          |
| R4   | 75R   |Resistor| 0603 |                          |
| R5   | 75R   |Resistor| 0603 |                          |
| R6   | 75R   |Resistor| 0603 |                          |
| R7   | 75R   |Resistor| 0603 |                          |
| R8   | 10K   |Resistor| 0603 |                          |
| J1   |       |Connector| DB23M | D-Sub Male             |
| J2   |       |Connector| DB15F | D-Sub Female Hi Density|
| J3   |       |Connector| MD-60SV | 6 Pin Mini DIN       |
| J4   |       |Connector| DB9F  | D-Sub Female           |
| J5   |       |Connector| CP-3523SJR-ND | SMD 3.5mm Jack |
| J6   |       |Header| 2.54mm Male 1x06  | PIC ICSP      |
| J7   |       |Header| 2mm Male 2x05 | Video Breakout    |
| JP1  |       |Header| 2.54mm Male 1x03 | Sync Select    |

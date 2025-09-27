!Typical MCU Block Diagram

| CONTAINS          | ROM              | RAM              | CONTAINS          |
|-------------------|------------------|------------------|--------------------|
| PROGRAM           |                  | TEMPORARY DATA   |                    |
| EXECUTES PROGRAM   | CPU              |                  |                    |
| MANAGES EVENTS    |                  |                  |                    |
| SIGNAL GENERATION  | TIMER            |                  |                    |
| EVENT COUNTING    | APPLICATION TIME BASE |              |                    |
| EEPROM            | CONTAINS        | PERMANENT DATA   |                    |
| A/D CONVERTER     | ANALOG DATA     | ACQUISITION      |                    |
| PERIPHERAL        | I/O PORT        | SERIAL INTERFACE | SENDS AND RECEIVES DATA |

### ROM (Read Only Memory)
ROM is usually used to store program instructions. ROM is the least expensive means of storing a program in a microcontroller, especially for high volume manufacturing.

----

**AN887/1100**
1/12
1
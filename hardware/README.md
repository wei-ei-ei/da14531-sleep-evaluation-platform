# Hardware Platform

## Base platform

Renesas DA14531 SmartBond TINY Module Development Kit:

- DA145xx DEVKT-P PRO-MB for power, debugging, programming and current measurement.
- DA14531 SMARTBOND TINY MODULE daughterboard, PCB version 376-25-C.
- MikroBUS connector with I2C signals available by default.
- SWD, UART, reset, user LED and test points.

The development kit does not contain PPG, accelerometer, temperature or haptic sensors. External modules are required.

## Sensor modules

| Function | Reference module or part | Interface |
| --- | --- | --- |
| PPG | MAX30102 breakout module | I2C, address 0x57 |
| Motion | LIS2DW12 three-axis accelerometer module | I2C, address 0x18 or 0x19 |
| Temperature | MCP9808 module or Thermo 8 click | I2C, address configurable from 0x18 to 0x1F |
| Optional comparison | TMP117 module | I2C, address 0x48 to 0x4B |
| Firmware reference | ADXL345 module | I2C; useful for the official Renesas accelerometer example |

## Integration notes

- The default MikroBUS I2C mapping uses P0_11 for SDA, P0_8 for SCL and P0_7 for an interrupt.
- P0_11 is shared with the user button and P0_7 with UART RTS, so simultaneous functions must be checked.
- Use one I2C pull-up pair for the complete bus.
- Confirm the actual VCC level on the MikroBUS header before connecting a sensor.
- The exact daughterboard revision must be checked against the supplied schematic before wiring.

## Reference documents

The repository links to Renesas official hardware documentation rather than redistributing vendor manuals. See [the reference index](../references/README.md).

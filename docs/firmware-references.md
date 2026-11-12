# Firmware and SDK References

## Renesas SDK6

The project uses Renesas SmartBond SDK6 and the published example repository:

- <https://github.com/renesas/ble-sdk6-examples>

Relevant example areas:

| Topic | Example reference | Reusable concept |
| --- | --- | --- |
| Custom BLE service | `ble_app_peripheral` | Characteristic definitions, notifications and callbacks |
| Sleep mode | `ble_app_sleepmode` | Extended-sleep configuration |
| OTA | `ble_app_ota` | Firmware update framework |
| I2C | `peripheral_examples/i2c` | Bus initialization and transactions |
| Battery/ADC | `peripheral_examples/adc/batt_lvl` | ADC sampling and voltage conversion |
| Accelerometer | `interfaces/accel-Sensor` | I2C acquisition with BLE notifications |
| Temperature | `connectivity/ble_temperature` | Thermo 8 click and MCP9808 access |

## Proposed software modules

```text
application/
  ble_service/
  sensor_bus/
    ppg/
    imu/
    temperature/
  features/
    heart_rate/
    hrv/
    activity/
  power/
  storage/
  diagnostics/
```

## Toolchain

- Renesas SmartSnippets Studio and SDK6.
- Keil MDK or e2 studio, depending on the selected SDK6 project target.
- SEGGER J-Link support through the development kit.
- SmartSnippets Toolbox Power Profiler for current measurements.

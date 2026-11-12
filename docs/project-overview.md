# Project Overview

## Purpose

DA14531 Sleep Sensing Evaluation Platform demonstrates how an ultra-low-power BLE development kit can acquire physiological signals, extract compact features and transfer useful sleep information to a host device.

The project focuses on the signal and software path rather than a product enclosure. This makes the platform useful for evaluating sensors, BLE throughput, power states and sleep-analysis methods on a reproducible development board.

## Target users

- Embedded developers exploring DA14531 and SDK6.
- Researchers and students studying wearable sleep-sensing signals.
- Engineers evaluating PPG, accelerometer and temperature modules.
- Readers interested in an end-to-end BLE health-sensing demonstration.

## Planned outputs

- DA14531 firmware with documented sensor drivers and BLE services.
- A host application for live visualization and recording.
- A replay pipeline for raw signals and extracted features.
- Sleep-related feature reports with explicit quality indicators.
- Current-consumption measurements for different operating states.
- Public technical notes covering architecture and implementation.

## Design principles

- Keep physiological signals and derived features traceable to one timestamped data model.
- Separate raw diagnostics from the lower-rate production feature stream.
- Record data quality instead of hiding missing or motion-corrupted segments.
- Make every result reproducible from recorded data.
- State the limits of consumer and research-grade sleep sensing clearly.

## Non-goals

- Clinical diagnosis or treatment.
- Regulatory certification.
- Claimed medical accuracy for sleep stages, heart rate or oxygen saturation.
- Presenting development-board results as a commercial wearable product.

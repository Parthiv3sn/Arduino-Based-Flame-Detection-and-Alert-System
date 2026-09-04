# Arduino-Based-Flame-Detection-and-Alert-System

A simple local fire-alert prototype that monitors a digital flame sensor and activates a visual and audible alert when a flame is detected.

> This is an educational prototype, not a certified fire-safety device. Do not use it as the sole protection for people or property.

## Features

- Reads a digital flame sensor
- Activates an LED and buzzer on detection
- Streams sensor state over serial at 9600 baud

## Hardware

- Arduino Uno or compatible board
- Digital flame sensor module
- LED with current-limiting resistor
- Buzzer

## Wiring

| Function | Arduino pin |
| --- | --- |
| Flame-sensor digital output | 9 |
| LED | 8 |
| Buzzer | 7 |

The current code treats a **LOW** sensor reading as flame detected. Confirm this behavior with your sensor module before use.

## Setup

1. Open `Source Code` (rename it to `FlameAlert.ino` if needed).
2. Wire the sensor, LED, and buzzer.
3. Upload and view serial output at **9600 baud**.

## Project files

- `Source Code` — Arduino sketch
- `Circuit Image .png` — wiring reference

## Improvement ideas

- Add sensor calibration and noise filtering.
- Add a test button and alarm-latch/reset behavior.
- Send alerts through a supervised communication channel.
- Use a certified smoke/fire alarm for real safety-critical deployments.

## License

No license has been specified. Add one before reusing or distributing this work.
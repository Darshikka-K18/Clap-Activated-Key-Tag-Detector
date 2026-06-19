# Clap-Activated Key Tag Detector

## Overview

Designed and implemented a battery-powered key tag finder that helps locate misplaced keys using acoustic triggers. The device listens for a specific audio pattern—two claps occurring within a 3-second window—and outputs an audible tone in response. The tone sounds for a short duration before the system automatically resets itself to standby mode.

A major engineering constraint of this project was achieving the time-window logic and tone generation **exclusively using 555 Timer ICs**, completely avoiding the use of microcontrollers or dedicated logic gate ICs.

## Key Features

* **Acoustic Activation:** Triggers an audible location tone upon detecting a double-clap audio pattern.
* **Time-Window Logic:** Successfully implements a 3-second timing window for the double-clap detection using purely analog/timer-based circuitry.
* **Auto-Reset Mechanism:** The alarm tone sounds for a predefined short duration before automatically resetting and returning to a low-power listening state.
* **Pure 555 Timer Architecture:** The entire control logic, timing, and tone generation were built using only 555 timer integrated circuits.
* **Battery Powered:** Designed for low power consumption suitable for a portable key tag device.

##  Development Workflow

1. **Circuit Design:** Logic and timing networks calculated for standard 555 timer configurations (monostable and astable modes).
2. **Simulation:** The complete circuit behavior was fully modeled and verified using **Proteus Design Suite**.
3. **Hardware Prototype:** Successfully built and hardware-tested on a physical breadboard to validate acoustic sensitivity and timing accuracy.

### Breadboard Prototype
![Working Breadboard Prototype](./Media.jfif)

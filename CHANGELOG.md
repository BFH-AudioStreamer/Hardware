# Changelogs

## Overview

- [Carrier-Board Apalis](#carrier-board-apalis)
- [Carrier-Board DAC](#carrier-board-dac)
- [DAC AK4493 Dual](#dac-ak4493-dual)
- [Encoder](#encoder)
- [Filter SallenKey](#filter-sk)
- [Isolator Mangetic](#isolator-mangetic)
- [Power Supply Unit](#psu)
- [Mainboard (discontinued)](#mainboard-discontinued)



## Carrier-Board Apalis

### V1.1 2019-09-09

#### Added
- Toradex Apalis carrier-board sections from [Mainboard 1.0](#mainboard-discontinued)
- Power off signal to CoM
- USB OTG interface for CoM flash access

#### Modified
- USB micro replaced by USB C connectors
- Fix footprint of HDMI2C1-6C1
- Fix schematic library error of M.2 Type B

#### Removed
- CoM signal LEDs



## Carrier-Board DAC

### V1.1 2019-09-09

#### Added
- DAC and power supply section from [Mainboard 1.0](#mainboard-discontinued)
- 0.1" connectors for DAC and filter modules

#### Modified
- Fix schematic library error of LT3094
- Fix overvoltage on voltage supervisor with voltage divider



## DAC AK4493 Dual

### V1.1 2019-09-09

#### Added
- DAC section from [Mainboard 1.0](#mainboard-discontinued)
- 5V voltage reference
- 0.1" connectors

#### Removed
- Reconstruction filter

## Encoder

### V1.0 2019-05-09

#### Added
- Rotary encoder with button
- 6 blue LEDs



## Filter SK

### V1.1 2019-09-09

#### Added
- Sallen-Key filter section from [Mainboard 1.0](#mainboard-discontinued)
- 0.1" connectors

#### Modified
- OPAMP footprint: SMD to DIP/SMD

#### Removed
- DC bias compensation



## Isolator Mangetic 

### V1.1 2019-09-09

#### Added
- Digital isolator section from [Mainboard 1.0](#mainboard-discontinued)
- 0.1" connectors

#### Modified
- SOIC wide footrpints replaced by SOIC narrow
- Fix pin mixup on the isolators

#### Removed
- Crystal oscillators



## PSU

### V1.0 2019-05-09

#### Added
- Analog power supply based on transformer, rectifier, caps
- Analog supply control with solid state relay (OptoMOS relay)
- Digital power supply based on AC/DC module

### V1.1 2019-09-09

#### Modified
- Fix schematic library error of CPC1926Y

## Mainboard (discontinued)

### V1.0 2019-05-09

#### Added
- Toradex Apalis carrier board based on the [Toradex Ixora source files](https://developer.toradex.com/products/ixora-carrier-board#design-resources)
- Net classes for high-speed signals
- Backlight control for parallel display output 
- Dual AK4493 DAC output
- Sallen-Key reconstruction filter
- Analog power supply with low noise linear regulators
- Digital signal isolation with magnetic low noise isolators
- Crystal oscillators for low jitter clock sources (22.5792 MHz and 24.5760 MHz)

#### Modified
- Apalis carrier board:
    - Minimal footprint size 0603 (imperial)
    - Altium project hierarchy changed from busses and labels to harnesses
    - Replaced obsolete components
    - M.2 connectors instead of mini PCIe connectors
    - Vertical ethernet connector instead of horizontal
    - Virtual COM port over USB instead of RS-232

#### Removed
- Apalis carrier board:
    - Fan control
    - Board ID EEPROM
    - SD card slot
    - Analog audio output
    - Camera interface
    - Resistive touch interface
    - LVDS display connector
    - CAN bus interface
    - Extension connector
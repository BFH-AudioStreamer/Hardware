# Changelogs

## Overview

- [Carrier-Board Apalis](#carrier-board-apalis)
- [Carrier-Board DAC](#carrier-board-dac)
- [Encoder](#encoder)
- [Filter-SK](#filter-sk)
- [Isolator Mangetic](#isolator-mangetic)
- [Power Supply Unit](#PSU)
- [Mainboard](#mainboard) (discontinued)


## Carrier-Board Apalis


## Carrier-Board DAC


## Encoder
### 1.0 2019-05-09
#### Added
- Rotary encoder with button
- 6 blue LEDs

## Filter-SK


## Isolator Mangetic 


## Mainboard (discontinued)
### 1.0 2019-05-09
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

## PSU
### 1.0 2019-05-09
#### Added
- Analog power supply based on transformer, rectifier, caps
- Analog supply control with solid state relay (OptoMOS relay)
- Digital power supply based on AC/DC module


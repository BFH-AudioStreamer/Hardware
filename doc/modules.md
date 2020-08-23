# Modules

The streamer was divided into several modules (PCBs) to be able to change to your favourite DAC or filter. But foremost to test and compare different circuit designs and component. The module groups are shown below.

## Carrier Board

A carrier board contains a socket for a module, as well as connectors for internal or external usage. They also contain the voltage regulators to supply the module.

Currently there are two carrier boards: on for the computer on a module (Toradex Apalis iMX6) and the digital to analog converter. With these two carrier boards the noisy digital and the sensitive analog circuits are separated.

## DAC

The DAC module contains an audio DAC with its circuitry. The performance of different DACs can be tested this way. Currently there exists a DAC module containing two AK4493 DACs.

## Filter

Every DAC needs a reconstruction filter. There are lots of operational amplifiers and different circuit designs available. To accommodate for the different performances the filter circuit can be swapped with a module.

## Isolator

To isolate the noisy digital circuit from the analog circuits a isolator module can be used.

## Power supply

The power supply converts mains AC to intermediate DC voltages for the carrier boards.

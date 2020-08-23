# Concept

The concept was created for standalone streamer with a touch-screen interface.

![Concept](img/Concept-Block-Diagram.svg)

## Power Supply

The streamer can be divided into two main sections: a noisy computer section and a sensitive analog section containing the DAC. To isolate noise from the sections they are galvanically isolated.

The mains power is filtered with feed through filter to remove noise from mains. The filter AC signal is fed to a AC/DC module for the computer section and converted to DC in the analog section with a transformer/rectifier circuit. The transformer circuit with following linear regulators should result in a low noise DC supply for the DAC. A linear regulator for the computer is not feasible, due the high power consumption (ca. 5W).

## Digital/Analog Converter

The DAC is powered from a clean power supply. The digital audio stream can be sourced from I2S. The control the DAC I2C or SPI can be used, depending on the DAC selection. As sigma delta DACs typically use the I2S MCLK as system clock, a jitter free clock should be provided. This is done by the low jitter oscillators which can be selected as MCLK.

The analog signal from the DAC is passed through a filter to remove aliasing effects. The main analog output of the device are the RCA connectors. However, as most DAC output a differential signal two XLR connectors are intended on the desing.


## Computer

A computer on a module (CoM) is used to stream audio from the internet to the DAC. This prototype is based on an Apalis iMX6Quad module from Toradex. Therefore the computer section consists of the carrier board for this module.

To establish an connection to the internet ethernet and WiFi are intended. Local playback is possible over a USB interface. As the CoM also features a PCIe interface an SSD can be used as audio storage.

The streamer can be configured in standalone or server mode. In standalone mode the user can choose and control the audio playback directly on the device. A touch-screen interfaced by parallel-RGB and I2C or HDMI and USB can be used for that purpose.

## Isolation

The whole design is split into three seperate parts: the mains (230V), analog and digital section. The sections are galvanically isolated to minimize the influence between each ohter. To isolate the signals between the computer and the DAC a digital isolator can be used.

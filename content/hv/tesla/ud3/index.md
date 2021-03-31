+++
title = "UD3"

[menu.main]
identifier = "ud3"
parent = "tesla"
weight = 10
+++

{{< imgproc "images/PXL_20210308_172554884.jpg" Resize "x200" "" "link" >}}

## Links

* [UD3 Altium schematic/pcb](https://github.com/Netzpfuscher/UD3_PCB)
* [UD3 firmware](https://github.com/Netzpfuscher/UD3)
* [Teslaterm](https://github.com/Netzpfuscher/Teslaterm)
* [Fiber ethernet schematic/pcb](https://github.com/TMaxElectronics/UD3_Fibernet)
* [Fiber ethernet firmware](https://github.com/TMaxElectronics/UD3-Fibernet-Firmware)
* [UD3 wiki](https://github.com/Netzpfuscher/UD3/wiki)

## Wiring diagrams

{{< imgproc "images/PXL_20210308_172545905.jpg" Resize "x400" "" "link" >}}

## Getting started

* prereqs
  * git
  * npm/nodejs
  * SMD soldering
  * basic IP networking
* ud3 and fibernet gerber files
* digikey BOMs/carts
* external parts
  * enclosure
  * dc power supply
  * hall effect DC CT
  * voltage divider resistors
  * GDT and FB cores
* ud3 assembly notes
* cypress kitprog programmer upgrade (for use with linux acm driver), setup, and usage
* compiling firmware with cypress designer
* flash firmware
* first connection over usb serial
  * linux serial config
* ud3 configuration
* usb->uart converter wiring and usage
* teslaterm build/run
* fibernet
  * {{< imgproc "images/PXL_20210320_172427435.jpg" Resize "x200" "" "link" >}}
  * media converters
  * SFPs
  * MM fiber
  * dhcp server / network config

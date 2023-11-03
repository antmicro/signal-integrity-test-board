# Antmicro's Signal Integrity Test Board

Copyright (c) 2023 [Antmicro](https://www.antmicro.com)

![Signal Integrity Testboard](/img/si-testboard-vis.png)

## Overview

This project contains open hardware design files for a test board implementing various routing topologies.
The board can be used for calibrating and comparing measurements of signal propagation properties with Vector Network Analyzers (VNA's).
It can also be used for doing SI, EMI, EMC simulations with field solvers.
The board was designed in KiCad 6.x.

## Project structure

The main directory contains the KiCad design files, LICENSE and README.
The remaining files are stored in the following directories:

* ``img`` - contains graphics for this README
* ``doc`` - contains generated schematics and other documentation
* ``lib`` - contains KiCad component library
* ``assets`` - contains visual content used for showcasing the board at [Open Hardware Portal(https://openhardware.antmicro.com)

## Key features

* 4-layer PCB designed in defined impedance
* Includes SMA ports connected to copper primitives which implement the following features:

  * VNA calibration port terminated with 50Ohm
  * VNA calibration port open (i.e. not terminated)
  * VNA calibration port shorted (grounded) 
  * Single stripline
  * Differential pair stripline
  * Stripline with long stub
  * Stripline with short stub
  * Digital bandpass filter
  * Reference stripline layout with layer-change
  * Simple planar antenna
  * Not-terminated striplines with tight and loose meander of the same lengths

## License

This project is licensed under the [Apache-2.0](LICENSE) license.

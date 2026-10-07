# USB-C 5V Power Supply PCB

## Project Overview

This project presents the design and PCB implementation of a compact USB-C 5V power supply using KiCad.

The design accepts 5V power through a USB-C connector and provides a protected and filtered 5V output. The PCB includes input protection, decoupling capacitors, transient voltage protection and USB-C CC resistors.

## Features

- USB-C 5V power input
- 5V power output interface
- USB-C CC1 and CC2 pull-down resistors
- 500 mA resettable fuse for input protection
- TVS diode for transient voltage protection
- Input/output filtering capacitors
- Two-layer PCB design
- Ground copper zone
- Design Rule Check (DRC) completed
- Gerber and drill fabrication files generated
- 3D PCB model verified in KiCad

## Main Components

| Reference | Component | Function |
|---|---|---|
| J1 | USB-C Receptacle | 5V power input |
| F1 | 500 mA Polyfuse | Overcurrent protection |
| R1 | 5.1 kΩ | USB-C CC1 pull-down |
| R2 | 5.1 kΩ | USB-C CC2 pull-down |
| C1 | 10 µF | Power filtering |
| C2 | 10 µF | Power filtering |
| D1 | SMBJ5.0A TVS | Transient voltage protection |
| J2 | 2-pin connector | 5V output |

## Design Flow

1. Circuit schematic design
2. Component selection
3. PCB footprint assignment
4. PCB placement
5. PCB routing
6. Ground copper zone implementation
7. Design Rule Check (DRC)
8. 3D PCB verification
9. Gerber generation
10. Drill file generation

## PCB Design

The PCB was designed as a two-layer board using KiCad.

The main design considerations were:

- Short power-current paths
- Appropriate component placement
- Ground-plane connectivity
- USB-C connector routing
- Protection component placement
- Manufacturable PCB layout

## Verification

The PCB was checked using KiCad Design Rule Check (DRC).

*The PCB was checked using KiCad Design Rule Check (DRC), and electrical connectivity was verified with 0 unconnected items.*

The completed PCB was also inspected using KiCad 3D Viewer.

## Fabrication Files

The `Gerbers` folder contains the manufacturing files required for PCB fabrication, including:

- Front copper
- Back copper
- Front solder mask
- Back solder mask
- Front silkscreen
- Back silkscreen
- Board Edge Cuts
- Gerber job file
- PTH drill file
- NPTH drill file

## Software Used

- KiCad 10.0
- KiCad Schematic Editor
- KiCad PCB Editor
- KiCad 3D Viewer
- KiCad Gerber Viewer

## Repository Contents

```text
USB-C-5V-Power-Supply-PCB/
│
├── Gerbers/
│   ├── Gerber fabrication files
│   └── Drill files
│
├── project1_USB-C 5v Power Supply PCB.kicad_sch
├── project1_USB-C 5v Power Supply PCB.kicad_pcb
├── project1_USB-C 5v Power Supply PCB.kicad_pro
└── README.md

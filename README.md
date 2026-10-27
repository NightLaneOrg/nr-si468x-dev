# 📡 Night Ride - Si468x Module

Open-source DAB/FM receiver module based on the **Silicon Labs / Skyworks Si468x series**.

This project provides hardware, software, and documentation to integrate a modern digital radio receiver into automotive and embedded Linux systems.

---

## Overview

The Si468x is a highly integrated broadcast receiver supporting:

- **DAB / DAB+**
- **FM (RDS)**
- Digital audio output via **I2S**
- Control via **I2C**

This repository focuses on building an **open and reusable platform** around the chip.

---

## Features

- Custom **M.2 E-Key module** design
- Automotive-oriented integration (infotainment systems)
- Linux driver / userspace control (WIP)
- Modular and reusable hardware design

---

## Repository Structure

```
/pcb        -> KiCad schematics & PCB layouts
/driver     -> Linux driver / interface code (WIP)
/tools      -> debugging and testing utilities
/firmware   -> placeholder (not included, see below)
```

---

## ⚠️ Firmware Notice

The Si468x requires proprietary firmware provided by the vendor.

❌ Firmware is **NOT included** in this repository  
❌ Redistribution is **not permitted**

See [`/firmware/README.md`](firmware/README.md) for details on how to obtain and use firmware.

---

## Hardware

> [!CAUTION]
> The PCBs till at least Commit ``9c4ef1d`` have I2S interferance issues, as is to hear [here](https://hut9.de/radio_audio)  
> This may have been fix in the later commits, but i don't have an later revision to this point
> so assume I2S will sound like that!  
> If someone knows how to fix that, feel free to contact me.

current design goals:

- Si4689-based RF frontend
- M.2 E-Key form factor
- External antenna support
- I2S digital audio output
- I2C host interface

[View Schematic & PCB](https://hut9.de/pcbs/nr-si468x-dev/)<br>
[View Schematic & PCB for the RPi adapter Hat](https://hut9.de/pcbs/nr-si468x-rpi-adapter/)

---

## Software

Planned features:

- Linux integration (userspace or kernel driver)
- Station tuning and service selection
- DAB / FM metadata parsing
- Integration into infotainment systems

---

## Documentation

Due to licensing restrictions, some vendor documentation is not included.

You may need to obtain:
- Programming guides
- Firmware files
- Additional application notes

These are typically available via:
- Community forums
- Existing development kits

---

## Status

🚧 Work in progress

- PCB: finished
- Driver: pending
- Testing: pending

---

## Licensing

This repository contains multiple components under different licenses:

- **Software (`/driver`, `/tools`)**  
  Licensed under the GNU General Public License v3.0 (GPL-3.0)

- **Hardware (`/pcb`)**  
  Licensed under the CERN Open Hardware License v2 - Strongly Reciprocal (CERN-OHL-S-2.0)

- **Firmware**  
  Not included. Proprietary and subject to vendor licensing.

See the individual folders for more details.

---

## 🌙 Night Lane

Part of the Night Lane open-source automotive platform.

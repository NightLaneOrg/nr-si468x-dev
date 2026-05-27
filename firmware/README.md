# Firmware

⚠️ The Si468x requires proprietary firmware which is **not included** in this repository.

## Why is firmware not included?

The firmware is:
- Proprietary
- Distributed under restrictive licenses
- Not legally redistributable

Including it in this repository would violate licensing terms.

---

## How to obtain firmware

You may be able to obtain firmware by:

- Contacting Skyworks (formerly Silicon Labs)
- Using official evaluation kits or SDKs
- Searching community forums and discussions

Example (unofficial, may change or disappear):

https://www.mikrocontroller.net/topic/342689

https://github.com/silelis/MustangRadio_develepementVersion/tree/main/02_Firmware/04_si468x

---

## Usage

Place firmware files in this directory:

```
firmware/
├── dab_radio_*.bin
├── fmhd_radio_*.bin
└── rom_patch*.bin
```

The software/driver will load firmware from this location.

---

## Disclaimer

This project does not provide or distribute firmware.

Users are responsible for ensuring they comply with all applicable licenses.

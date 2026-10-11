# Geeetech A20M Marlin firmware (my config)

I've upgraded the original printer with:

- TMC2208 Drivers
- Nema 17 rubber dumpers
- Noctua NF-A4x10 FLX fans for 
- GELID Silent 5 fan
- PC4-M6 connectors
- PTFE blue tubes
- E3D V6 hotend (replaced a Chimera 2in 2out, which gave poor results)
- Geeetech 3D Touch V3.2

## Firmware

- `A20M_Marlin_2.1.2.8`: current firmware, Marlin 2.1.2.8 based on the official
  [Geeetech/A20M example config](https://github.com/MarlinFirmware/Configurations/tree/release-2.1.2.8/config/examples/Geeetech/A20M).
- `A20M_Marlin_2.0.9.5`: previous firmware, kept for reference.
- `A20M_Marlin-1.1.x12864`: original Marlin 1.1.x firmware.

Build and flash (PlatformIO, board connected over USB), from the firmware folder:

```
pio run -e mega2560 -t upload
```

## Board

- Geeetech GT2560 V3.1 ([official schematic](https://github.com/Geeetech3D/Diagram/blob/master/GT2560_V3.0_SCH.pdf), V3.0, same layout)
- Connector pinouts and the bed thermistor rewiring: [docs/GT2560_V3.1_pinout.md](docs/GT2560_V3.1_pinout.md)
- The bed thermistor is wired to `EXT2` (pins 11-12) instead of `HB`, after the original input was damaged by a short.

Useful links::

- https://github.com/Geeetech3D/Prusa_I3_3Dprinter
- https://marlinfw.org/docs/configuration/configuration.html
- https://marlinfw.org/docs/hardware/tmc_drivers.html
- https://github.com/MarlinFirmware/Configurations/tree/release-2.1.1/config/examples/Geeetech/A20M

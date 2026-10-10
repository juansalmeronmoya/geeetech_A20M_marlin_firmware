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

## Board

- Geeetech GT2560 V3.1 ([official schematic](https://github.com/Geeetech3D/Diagram/blob/master/GT2560_V3.0_SCH.pdf), V3.0, same layout)
- Connector pinouts and the bed thermistor rewiring: [docs/GT2560_V3.1_pinout.md](docs/GT2560_V3.1_pinout.md)
- The bed thermistor is wired to `EXT2` (pins 11-12) instead of `HB`, after the original input was damaged by a short.

Inspired on:

- https://github.com/Geeetech3D/Prusa_I3_3Dprinter
- https://github.com/MarlinFirmware/Configurations/tree/import-2.0.x/config/examples/Geeetech

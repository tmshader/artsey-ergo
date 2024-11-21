# Artsey Ergo
A 3D printable ergonomic wireless Artsey-based keyboard running ZMK.

## Features:
- NRF52840 chip for fast communication over BLE
- USB-C for charging, updating and communication instead of BLE
- Slightly modified Artsey 9.0.0 layout
- 128x32 OLED display for layers, battery status, time and other fun stuff

## Try and modify the project

Modify `ergogen/config.yaml` or use the provided config.

Run ergogen to create the base files:
```bash
ergogen ./ergogen -o .
```

This creates an `outlines` and a `pcbs` folder:
- The `pcbs` folder contains the starting point from which we can start routing and modifying the board.
- The `outlines` folder contains a bunch of mechanical drawings in `.dxf` format but the most important for us is `cad.dxf` which we can import into our favourite CAD software (Fusion, FreeCAD, Solidworks, etc.) and start designing a case for the keyboard.

## Upcoming changes
- Production ready PCBs
- Choc and MX compatible board versions
- A case for 3D printing and one for CNC machining
- Using the NRF52840 chip instead of a module
- Thread and Zigbee support (why not?)
- OTA Updates
# Notecarrier-Micro

This folder contains the design files for the Blues Wireless Notecarrier-Micro, in KiCad 7 format. This is a compact carrier board designed specifically for the Blues Wireless Notecard, providing power management, interface conversion, and mechanical mounting in a minimal form factor.

The Notecarrier-Micro provides essential hardware interfaces including USB-C for programming and power, JST connectors for battery and antenna connections, and standard 0.1" headers for GPIO access. All components are selected for low power consumption and reliability in IoT applications.

## Contents

- This file
 	- `README.md`
- KiCad source files
	- `Notecarrier-Micro.kicad_pcb`
	- `Notecarrier-Micro.kicad_prl`
	- `Notecarrier-Micro.kicad_pro`
	- `Notecarrier-Micro.kicad_sch`
	- `Notecarrier-Micro.kicad_wks`
	- `sym-lib-table`
	- `fp-info-cache`	- `fp-lib-table`
- Documentation	- `documentation/*`
- Manufacturing artefacts
	- `manufacturing/*`
- Design references
	- `reference/*`
- Validation artefacts
	- `validation/*`


## Hardware Specifications

### Physical Characteristics
- **Dimensions**: Compact form factor optimized for space-constrained applications
- **Mounting**: Standard mounting holes for secure installation
- **Connectors**: USB-C, JST battery connector, antenna connectors, 0.1" GPIO headers

### Power Management
- **Input Voltage**: USB-C 5V input, Battery input via JST connector
- **Power Regulation**: On-board voltage regulators for stable 3.3V and other required voltages
- **Low Power Design**: Optimized for battery-powered IoT applications

### Interfaces
- **USB-C**: Programming, debugging, and power input
- **Battery Connector**: JST connector for LiPo battery connection
- **Antenna Connectors**: Standard antenna connections for cellular/WiFi
- **GPIO Headers**: 0.1" pitch headers for external sensor/actuator connections
- **I2C/SPI/UART**: Standard communication interfaces exposed via headers

### Compatibility
- **Notecard Support**: Designed specifically for Blues Wireless Notecard modules
- **Module Interface**: M.2 edge connector for Notecard installation
- **External Access**: All Notecard pins accessible via expansion headers

## Manufacturing Files
- **PCB Files**: Complete KiCad manufacturing package in `manufacturing/` directory
- **3D Models**: STEP and WRL files for mechanical integration
- **Assembly**: Pick and place files, BOM, and assembly drawings

## Revision History

| Revision |    Date    |   Author   | Description |
|:--------:| ---------- | ---------- | ----------- |
|     A    | 2023-03-31 | H.Raftery  | initial port from OrCAD design files, rev 14 (v2.1). |


### Original OrCad Design File Revision History

| Revision |    Date    |   Author   | Description |
|:--------:| ---------- | ---------- | ----------- |
|    12    | 25/08/2020 | G.Boschini | - Changed screw with inox version<br/>- Changed pullup resistor of EN pin to 10M |
|    14    | 25/08/2020 | M. Gregis  | - Added LiPO charger<br/>- Changed V+ to VBAT<br/>- removed BOOT signal from J21 header and replaced with GND<br/>- removed AUX5 from J22 header and replaced with VMODEM |

# Dell Inspiron 5548 MacOS Sonoma EFI (with bare essential kexts working):

## System Specifications:

- Intel Broadwell(5th gen) i5-5200U @ 2.20GHz.
- RAM: 16 GB DDR3-SDRAM.
- iGPU: Intel HD Graphics 5500.
- dGPU: AMD Radeon R7 M265.
- Storage: SSD 500 GB.

## EFI Specifications:

- Opencore v0.9.1
- Debug version and Release version both in separate branches

## Kexts:

- Airportitlwm (Wifi: Sonoma 14.5 version)
- AppleALC (Audio: Not working)
- ECEnabler (For Battery)
- Lilu (required for many processes to work properly)
- SMC (includes all kexts for SMC to work properly)
- VoodooPS2Controller (For keyboard and touchpad)
- WhateverGreen (Graphics: Accelaration not working)

## ACPI:

- SSDT-EC-Laptop
- SSDT-PLUG
- SSDT-PLNF
- SSDT-XOSI

## Not Working (Please open PR as this is a public repo):

- Bluetooth
- Audio
- Hardware Accelaration (especially need for graphics)

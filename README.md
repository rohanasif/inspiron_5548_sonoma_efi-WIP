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

## Not Working (Please open a PR as this is a public repo):

- Bluetooth
- Audio
- Hardware Accelaration (especially need for graphics)
- Other minor issues like volume controls and brightness controls

## PR and Forking:

- Open a PR or Fork if you like to improve this project.
- After you add features, please remove all verbose and debugging logs so that a clean EFI remains. Use release versions of both OpenCore and Kexts and remove the -v flag from boot-args in config.plist.
- Also please use GENSMBIOS from corpnewt on github, to generate your own SMBIOS for iMac19,1. As I already have the one in the current plist working on my pc so it won't work.

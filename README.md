# EFI-X99-MACHINIST-RS9-RX6600
- EFI for Motherboard Machinist X99-RS9 \
[![MacOS version](https://img.shields.io/badge/Monterey-12.7.1-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Ventura-13.6.2-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Sonoma-14.2-informational.svg)](https://www.apple.com/macos) \
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.9.7-informational.svg)](https://github.com/acidanthera/OpenCorePkg)

## This EFI Supports Hackintosh since Monterey version 12.3.1

## Hardware Specifications

| Component        | Model                                              |
| ---------------- | ---------------------------------------------------|
| Platform         | LGA 2011-3 - Intel Xeon V3                         |
| CPU              | Intel Xeon E5-2660 v3, 2600 MHz (10C/20T)          |
| MotherBoard      | MACHINIST X99-RS9                                  |
| Wifi             | Fenvi FV-AC1200                                    |
| OS Disk          | SSD NVMe Asgard AN 3.0 1TB                         |
| RAM              | 4x 8gb Asgard Valkyrie V5 32GB Ram                 |
| GPU              | AMD Radeon RX6600 (8 GB)                           |
| Cooler    	   | COOLER MASTER HYPER H412R                          |
| OpenCore   	   | 0.9.7          		                        |

## BIOS setup

**It is recommended to perform this configuration in case of a video card crash.**

- Turbo Boost Unlock: Yes / No

Disable:
- Fast Boot
- Secure Boot
- Serial/COM Port
- Parallel Port
- VT-d (can be enabled if you set DisableIoMapper to YES)
- Compatibility Support Module (CSM).
- Thunderbolt (For initial install, as Thunderbolt can cause issues if not set up correctly)
- Intel SGX
- Intel Platform Trust
- CFG Lock (MSR 0xE2 write protection) (This must be off; if you can't find the option, then ENABLE AppleXcpmCfgLock. Your hack will not boot with CFG-Lock enabled. For 10.10 and older, you'll need to ENABLE AppleCpuPmCfgLock as well.)

Enable:
- VT-x
- Above 4G decoding (This must be on; if you can't find the option, then add npci=0x2000 to boot-args. Do not have both this option and npci on boot-args enabled at the same time.)
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: Windows 8.1/10/11 UEFI Mode
- SATA Mode: AHCI

## Important informations

```bash
prev-lang:kbd: variable was set to value "pt-BR:128"
revcpuname: variable was set to value "Intel(R) Xeon(R) CPU E5-2660 v3 @ 2.60GHz"
(Optional) Download RadeonSensor for AMD GPUS: https://github.com/aluveitie/RadeonSensor
(optional) Download Stats (macOS system monitor in your menu bar): https://github.com/exelban/stats
```

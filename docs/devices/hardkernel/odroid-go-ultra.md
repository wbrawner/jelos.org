# Odroid Go Ultra

![](../../_inc/images/devices/hardkernel-odroid-go-ultra.png){ .off-glb }

## Overview

| Device | CPU / Architecture | Kernel | GL driver | Interface |
| -- | -- | -- | -- | -- |
| Odroid Go Ultra | Amlogic S922X / Mali G52 M6 (ARMv8-A) | Mainline Linux | Mali | Weston + Emulation Station |

## Features

| Feature&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Notes |
| -- | -- |
| :material-harddisk: Storage | JELOS should be installed directly to the internal EMMC. <br> When installed directly to the EMMC; an SD Card can be used for game storage. |

## Notes

### Installation

First download the latest `S922X-Odroid_GOU` version of JELOS from the button below.

[![Latest Version](https://img.shields.io/github/release/JustEnoughLinuxOS/distribution.svg?labelColor=111111&color=5998FF&label=Latest&style=flat#only-light)](https://github.com/JustEnoughLinuxOS/distribution/releases/latest)
[![Latest Version](https://img.shields.io/github/release/JustEnoughLinuxOS/distribution.svg?labelColor=dddddd&color=5998FF&label=Latest&style=flat#only-dark)](https://github.com/JustEnoughLinuxOS/distribution/releases/latest)

There are 2 options for installing JELOS on the Odroid Go Ultra:
1. Install JELOS directly to the 16 GB onboard EMMC memory and use the microSD card slot for ROMS; or
2. Zero-fill the onboard EMMC memory, install JELOS to a microSD card and load ROMS / games onto the same microSD card.

Option 1 is recommended as it makes the most of available storage and allows separation of the operating system (on EMMC) and ROMS / games (on microSD). However Option 2 may come in handy if you would like to run different versions of JELOS installed to different microSD cards.

For either option, you will need to boot the Odroid Go Ultra into recovery mode. To do this, follow the steps on [the Odroid wiki](https://wiki.odroid.com/odroid_go_ultra/getting_started/installing_os_image#installation).

#### Option 1 - Install JELOS to EMMC
- Once booted in recovery mode and connected to a PC via USB-C, the JELOS image may be flashed to the EMMC using Balena Etcher, win32diskimager, dd or similar.
- Restart the device and JELOS will go through its first boot process (running from EMMC).

#### Option 2 - Zero-fill EMMC and install JELOS to microSD
- Once booted in recovery mode and connected to a PC via USB-C, EMMC may be zero-filled, perhaps using dd, for example `dd if=/dev/zero of=/dev/<emmc_device_node> bs=1M`.
- Write the JELOS image to a microSD card using dd or similar.
- Power off the device, insert the JELOS microSD card, power on the device and JELOS will go through its first boot process (running from microSD).

### Troubleshooting

You cannot brick this device. If you cannot get into recovery mode, do the following:

- Download [this recovery image](https://wiki.odroid.com/odroid_go_ultra/os_image/recovery).
- Follow the recovery steps on [the Odroid wiki](https://wiki.odroid.com/odroid_go_ultra/getting_started/recovery_emmc)

The device should now be in recovery mode, ready to flash JELOS (or other firmware) to the device.

## Additional References

- [Platform Documentation (S922X)](https://github.com/JustEnoughLinuxOS/distribution/blob/main/documentation/PER_DEVICE_DOCUMENTATION/S922X)
- [Odroid Go Ultra wiki](https://wiki.odroid.com/odroid_go_ultra/odroid_go_ultra)
# Loki Zero

![](../../_inc/images/devices/ayn-loki.png){ .off-glb }

## Overview

| Device | CPU / Architecture | Kernel | GL driver | Interface |
| -- | -- | -- | -- | -- |
| Loki Zero | AMD Athlon Silver 3050e (x86_64) | Mainline Linux | Radeonsi | Weston + Emulation Station |

## Features

| Feature&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Notes |
| -- | -- |
| :material-harddisk: Storage | JELOS can be run from an SD Card, USB Drive or installed directly to the internal NVME. <br> When installed directly to the NVME; an SD Card can be used for game storage. |
| :material-fan: Fan | Can be set globally, per system or per game. |
| :material-lightning-bolt-circle: TPD Limit | Can be set globally, per system or per game. |
| :material-lightbulb-on: RGB | Supports selecting from a set of colors or turning the RGB off (choice persists through reboots) <br> Does not support changing brightness or turning on other effects. |

## Notes

| DMI_SYS_VENDOR | DMI_PRODUCT_NAME |
| -- | -- |
| `ayn` | `Loki Zero` |

### Installation

Download the latest `AMD64` version of JELOS from the button below and follow the instructions listed on the [Install](../../../play/install/) page.

[![Latest Version](https://img.shields.io/github/release/JustEnoughLinuxOS/distribution.svg?labelColor=111111&color=5998FF&label=Latest&style=flat#only-light)](https://github.com/JustEnoughLinuxOS/distribution/releases/latest)
[![Latest Version](https://img.shields.io/github/release/JustEnoughLinuxOS/distribution.svg?labelColor=dddddd&color=5998FF&label=Latest&style=flat#only-dark)](https://github.com/JustEnoughLinuxOS/distribution/releases/latest)

### Booting from an SD Card

In order to launch JELOS from an SD card or a USB drive you will need to first change the boot order in the BIOS.  

During boot you can enter the bios by either (1) holding the left & right button that sit bellow the dpad and right analog stick OR (2) connecting an external keyboard and pressing the `del` key.  

In the bios; navigate to the `Boot` menu and then change the boot order to prioritize the SD card or USB Drive under `Boot Order Priorities`. Then go `Save & Exit` and select the Save Changes and Exit option.  This change will persist through all reboots.  If you want to boot into Windows simply remove the SD Card or USB drive.

### Changing the RGB 

In EmulationStation press the `Start` button to open the Main Menu.  Then select `System Settings` and scroll until you see `Device LEDS`.  Under that setting you can choose to turn RGB Off or select from a set of pre-defined colors.  The value you set will persist through all future reboots but note your RGB setting will only take effect after JELOS boots.

## Additional References

- [Platform Documentation (AMD64)](https://github.com/JustEnoughLinuxOS/distribution/blob/main/documentation/PER_DEVICE_DOCUMENTATION/AMD64)
- [Device Quirks](https://github.com/JustEnoughLinuxOS/distribution/tree/main/packages/hardware/quirks/devices/ayn%20Loki%20Zero)
- [Panel Rotation](https://github.com/JustEnoughLinuxOS/distribution/blob/main/packages/kernel/linux/patches/AMD64/002-display-quirks.patch)
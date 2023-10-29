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

Download the latest `S922X-Odroid_GOU` version of JELOS from the button below.

!!! note "JELOS must be flashed directly onto the Odroid Go Ultra rather than an SD card.  This is done by putting the device into recovery mode, [as explained here](https://youtu.be/X9wbPY5qf6o?t=1195)."

[![Latest Version](https://img.shields.io/github/release/JustEnoughLinuxOS/distribution.svg?labelColor=111111&color=5998FF&label=Latest&style=flat#only-light)](https://github.com/JustEnoughLinuxOS/distribution/releases/latest)
[![Latest Version](https://img.shields.io/github/release/JustEnoughLinuxOS/distribution.svg?labelColor=dddddd&color=5998FF&label=Latest&style=flat#only-dark)](https://github.com/JustEnoughLinuxOS/distribution/releases/latest)

### Troubleshooting

You cannot brick this device. If you cannot get into recovery mode, do the following:

- Download [this recovery image](https://wiki.odroid.com/odroid_go_ultra/os_image/recovery).
- Flash the image to a spare microSD card using Balena Etcher or similar.
- Remove the back cover of the device (four screws).
- Locate a small button on the back of the board (the side that's visible), near the right thumbstick.
- While holding down the small button, power on the device.

The device should now be in recovery mode, ready to flash JELOS (or other firmware) to the device.

If you find yourself doing this often, consider drilling a pinhole in the back cover so that the button can be accessed with a paperclip.

![](../../_inc/images/devices/mods/powkiddy-rgb10max3pro-mod1.png){ .off-glb }

## Additional References

- [Platform Documentation (S922X)](https://github.com/JustEnoughLinuxOS/distribution/blob/main/documentation/PER_DEVICE_DOCUMENTATION/S922X)
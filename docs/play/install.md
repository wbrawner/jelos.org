# Installing JELOS

## Installation
* JELOS is installed by restoring an image file and [Flashing](https://github.com/JustEnoughLinuxOS/distribution/tree/main#flashing) to a device's internal storage or an external sd card.
* On x86 devices JELOS includes an installation tool.  The installation tool can be found in the tools menu, which is one of the systems listed within ES.
* JELOS operating system is stored on an Ext4 partition that can be read by LINUX but is not natively readable on Windows. Currently it is not possible to access the primary JELOS Ext4 partition on Windows to transfer roms.
* On devices that support a second sd card, the sd card can be formatted as Ext4, FAT32, or exFAT. JELOS will automatically detect the second SD card on boot and configure the relevant folders for storing roms.
* External services are disabled by default in release builds.  When enabled, the username for ssh and samba access is "root".  The root password is generated during every boot, it can be found in the System Settings menu.

## Flashing
* Download the latest [version of JELOS](https://github.com/JustEnoughLinuxOS/distribution/releases) (.img.gz) for your device.
* Decompress the image.
* Write the image to an SDCARD using an imaging tool.  Common imaging tools include [Balena Etcher](https://www.balena.io/etcher/), [Raspberry Pi Imager](https://www.raspberrypi.com/software/), and [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/).  If you're skilled with the command line, dd works fine too.
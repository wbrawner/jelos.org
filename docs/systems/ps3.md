# Sony Playstation 3

## Overview

| Path(s) | Supported Extensions |
| --- | --- |
| `storage/roms/ps3` | `.ps3` `.bin` |

## Emulator(s)

| Name | Documentation |
| --- | --- |
| RPCS3 | [rpcs3.net/quickstart](https://rpcs3.net/quickstart) |

## Instructions

!!! note "RPCS3 requires official PS3 firmware and due to that it requires additional set up before you can use it"

PS3 firmware cannot be installed directly through JELOS so you will need access to another computer where you have RPCS3 installed to get things started.

From your source computer make a copy of the `dev_flash` folder from your RPSC3 install directory (this folder is automatically created by RPCS3 after you have installed offical PS3 firmware)

Upload the full contents of that `dev_flash` folder to `storage/roms/bios/rpcs3` on your JELOS device (note: you will need to create the `rpcs3` folder if this is your first time setting it up).  

Once complete your folder structure should be `/bios/rpcs3/dev_flash` and that folder should contain the full contents of the dev_flash folder from your source PC.

Now you can try booting a game from EmulationStation.

On first boot you will get the RPCS3 welcome screen. Its recommended to check the box in the bottom right labled "Do not show again" (this will stop this screen showing up for future launches).  Check the "I have read the Quickstart guide" box and then select the continue button that shows up at the bottom left of the screen. 

Your game should boot at this point.  If not please check that the contents of the dev_flash folder (1) match the copy from your source computer and (2) is uplaoded to the correct location listed above.
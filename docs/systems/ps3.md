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

### Firmware Setup

!!! note "RPCS3 requires official PS3 firmware to be installed through the emulator GUI before you can run games. Its recommended to have a mouse/keyboard plugged in for these steps."

1. Download the latest official PS3 firmware from Sony's [PS3 System Software](https://www.playstation.com/en-us/support/hardware/ps3/system-software/) page.  The downloaded file will be named `PS3UPDAT.PUP`
2. Transfer the `PS3UPDAT.PUP` file to `~/storage/roms/temp`.  If the `temp` folder does not exist then please create it (you will delete this file after you have installed it).
3. Navigate to the Tools system and then select ++"Start RPCS3"++ (this will open the RPCS3 GUI where you will install the firmware you downloaded above).
4. Select `File > Install Firmware.`
5. Navigate to `~/storage/roms/temp`, select `PS3UPDAT.PUP` and press `Open`

The firmware will be installed and then a window will open to process the needed files; please let this process complete.  Once complete you can close out RPCS3 and return to EmulationStation.

### Game Setup

PlayStation 3 games can come in a few different formats (common ones are disc-based and Digital "PSN" games). The steps for setting up a given game differ depending on its source format.

#### Disc-Based Games
*TBA*

#### Digital "PSN" Games
*TBA*

### Running a Game

Now you can try booting a game from EmulationStation.

On first boot you will get the RPCS3 welcome screen. Its recommended to check the box in the bottom right labled "Do not show again" (this will stop this screen showing up for future launches).  Check the "I have read the Quickstart guide" box and then select the continue button that shows up at the bottom left of the screen. 
# WPSD Nextion Screens

> This is a fork of the [WPSD Project](https://repo.w0chp.net/WPSD-DEV/WPSD_Nextion/) with custom simplex/duplex LH screen variants, published under the GPLv3.0 license. Please keep this in mind if you modify and republish this layout.

The WPSD Nextion repo is a set of Nextion HMI (source) and TFT (compiled) files for use with various TFT screens made by Nextion for WPSD-based hotspots and repeaters.

## Available Screens

### NX4024K032_WPSD_3.2_Nextion_simplex_LH — 3.2"

Simplex, LH variant. HMI source and compiled `.tft` file included, ready to install directly on your screen.

- Layout optimized for 3.2" screens, including one field for Last Heard
- With some modifications in WPSD, it's possible to also show radio ID data (Name, Country, City) for YSF and D-Star mode

Files: [HMI](HMI/NX4024K032_WPSD_3.2_Nextion_simplex_LH.HMI) · [TFT](TFT/NX4024K032_WPSD_3.2_Nextion_simplex_LH.tft)

### NX8048K050_WPSD_5.0_Nextion_HighSpeed_LH duplex — 5.0"

High Speed, Duplex, LH variant. HMI source and compiled `.tft` file included, ready to install directly on your screen.

- Layout optimized for 5" screens, including one field for Last Heard
- With some modifications in WPSD, it's possible to also show radio ID data (Name, Country, City) for YSF and D-Star mode
- This layout is built for High Speed mode — in the hotspot config, set "Layout Type" to `ON7LDS L3 HS`

Files: [HMI](<HMI/NX8048K050_WPSD_5.0_Nextion_HighSpeed_LH duplex.HMI>) · [TFT](<TFT/NX8048K050_WPSD_5.0_Nextion_HighSpeed_LH duplex.tft>)

> **Note:** The radio ID feature only works if you add `SendUserDataMask=0b00000111` to the Nextion driver section of your hotspot configuration.

## Installation

1. Use a microSD card no greater than 32 GB formatted as FAT32
2. Download the TFT file for your model of the Nextion screen
3. Copy the TFT file to the microSD card

    :bulb:  The only file on the card should be the TFT file

4. Insert the microSD card containing the TFT file into the Nextion screen

    :exclamation:  Ensure you power down the Nextion screen before inserting the microSD card

5. Power on the Nextion screen with recommended clean power as per its datasheet

6. Allow the Nextion device to upload the TFT file

    :information_source: The upload may take several minutes; a progress bar will show while the upload is running

7. After the upload succeeds, power off the Nextion screen

8. Remove the microSD card from the Nextion screen

9. *Optional*: Power on the Nextion as a test with recommended clean power as per its datasheet

10. Reattach the Nextion screen to your hotspot/repeater

## Credits / Software Used

* FLAGCODE from Rob van Rheenen, PD0DIB

## License

[GNU General Public License 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html)

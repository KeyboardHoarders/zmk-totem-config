<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="/docs/images/TOTEM_logo_brigt.svg">
    <source media="(prefers-color-scheme: light)" srcset="/docs/images/TOTEM_logo_dark.svg">
    <img alt="TOTEM logo font" src="/docs/images/TOTEM_logo_bright.svg" width="450">
  </picture>
</div>

# ZMK CONFIG FOR THE TOTEM SPLIT KEYBOARD

[Here](https://github.com/GEIGEIGEIST/totem) you can find the hardware files and build guide.
[Here](https://github.com/GEIGEIGEIST/qmk-config-totem) you can find the QMK config for the TOTEM.

TOTEM is a 38 key column-staggered split keyboard running [ZMK](https://zmk.dev/) or [QMK](https://docs.qmk.fm/). It's meant to be used with a SEEED XIAO BLE or RP2040.

![TOTEM layout](/docs/images/TOTEM_layout.svg)

<img width="911" height="1518" alt="my_keymap (22)" src="https://github.com/user-attachments/assets/cf64ad49-f5ff-4a50-a76b-4ff352f98e3f" />

## HOW TO USE

- Fork this repo
- `git clone` your repo to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- Adjust the `totem.keymap` file (find all the keycodes on [the ZMK docs pages](https://zmk.dev/docs/codes/))
- `git push` your changes to your fork
- On the GitHub page of your fork navigate to "Actions" and download the `firmware.zip` archive

## FLASHING FIRMWARE

1. Keep both halves powered on
2. Plug in the left half and press reset twice quickly. This will open a directory on your computer.
3. Drag and drop the settings reset file onto the left half
4. Unplug the left half and plug in the right, press reset twice quickly. This will open a directory on your computer.
5. Drag and drop the settings reset file onto the right half
6. Unplug the right half and plug in the left half again
7. Press reset twice
8. Drag and drop `totem_left-seeeduino_xiao_ble-zmk.uf2` onto the storage device
9. Unplug the left half and plug in the right
10. Press reset twice
11. Drag and drop `totem_right-seeeduino_xiao_ble-zmk.uf2` onto the storage device

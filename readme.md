## please clone to your own repo.  All pull requests will be denied as I use this for my shops keyboards and have a keymap and guide print out that goes with it.

To flash:
1.Download firmware in actions tab.

2.keep both halves powered on

3.plug in left half and press reset button twice quickly.  This will open up a directory on your computer.

4.drag and drop settings reset file onto left half

5.unplug left and plug in right side press reset twice quickly. This will open a directory on your computer.

6.drag and drop the settings reset file onto the right half

7.unplug right half and plug in left half again

8.press settings reset twice

9.drag and drop the totem left firmware file

10.uplug left and plug in right 

11.press reset twice

12.drag and drop the totem right firmware file.


<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/TOTEM_logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/TOTEM_logo_bright.svg">
  <img alt="TOTEM logo font" src="/docs/images/TOTEM_logo_bright.svg">
</picture>

# ZMK CONFIG FOR THE TOTEM SPLIT KEYBOARD

[Here](https://github.com/GEIGEIGEIST/totem) you can find the hardware files and build guide.\
[Here](https://github.com/GEIGEIGEIST/qmk-config-totem) you can find the QMK config for the TOTEM.

TOTEM is a 38 key column-staggered split keyboard running [ZMK](https://zmk.dev/) or [QMK](https://docs.qmk.fm/). It's meant to be used with a SEEED XIAO BLE or RP2040.


![TOTEM layout](/docs/images/TOTEM_layout.svg)



<img width="911" height="1518" alt="my_keymap (22)" src="https://github.com/user-attachments/assets/cf64ad49-f5ff-4a50-a76b-4ff352f98e3f" />



## HOW TO USE

- fork this repo
- `git clone` your repo, to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- adjust the totem.keymap file (find all the keycodes on [the zmk docs pages](https://zmk.dev/docs/codes/))
- `git push` your repo to your fork
- on the GitHub page of your fork navigate to "Actions"
- scroll down and unzip the `firmware.zip` archive that contains the latest firmware
- connect the left half of the TOTEM to your PC, press reset twice
- the keyboard should now appear as a mass storage device
- drag'n'drop the `totem_left-seeeduino_xiao_ble-zmk.uf2` file from the archive onto the storage device
- repeat this process with the right half and the `totem_right-seeeduino_xiao_ble-zmk.uf2` file.

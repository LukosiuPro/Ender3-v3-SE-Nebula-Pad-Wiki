# Setting up Nebula Pad

!!! info
    Some of the instructions here reference files you can download from the [Creality Downloads](https://www.creality.com/pages/download-creality-nebula-smart-kit) page for the Nebula Pad.

Before you can do a lot of cool stuff with the Nebula Pad, you need to install it first. While the official manual offers some help, it is not specific to the Ender-3 V3 SE, which can lead to odd errors.

Before installing the kit, you may want to print a bracket for the new Nebula Pad as it will not fit on the stock bracket. There is a bracket model at the downloads page. If you want something simpler, you can also print an [adapter](https://www.thingiverse.com/thing:6371800) that lets you mount the Pad on the stock bracket.

## Installing motherboard firmware
The default formware for the Ender-3 V3 SE is designed to work with the stock screen. The Nebula Pad will not connect to the printer until you update the printer's motherboard to firmware that works with the Nebula Pad.

!!! note
    You can use the files from usb drive that came with your nebula pad, but they may be outdated. It is recommended to use the files from the Creality Downloads site.

1. Turn off your printer.
2. Unplug old screen.
3. Open creality website and navigate to [nebula smart kit page](https://www.creality.com/pages/download-creality-nebula-smart-kit)
4. Under section "**Download Product Firmware**" click download button.
5. When download finishes extract the contents of the zip file.
6. Now grab the sd card that came with the printer and format. Check the formatting guide based on your system:
    - [Windows](../general/format-sd.md#windows)
    - [Linux](../general/format-sd.md#linux)
    - [Mac](../general/format-sd.md#mac)
7. Open extracted folder, find "**Ender3V3SE_firmware.bin**"
8. Rename it to firmware.bin
9. Copy file to formatted sd card.
10. Put the SD card into printer slot and wait **~5min**
11. Then turn off the printer
12. Pull out the SD card.
13. Connect nebula pad to the printer.
14. **IMPORTANT!** Make sure you don't have the sd card in it the printer and no USB attached to the nebula pad.
15. Turn on the printer, wait a bit, let it initialize.
16. Now you can follow the [Setting up nebula pad tutorial](#setting-up-nebula-pad)

## Setting up nebula pad
1. When you boot up for the first time, you will be greated with printer selection.
2. Based on version which your nebula pad came in, you will see arrows or buttons to go to next page of the list.
3. Find Ender 3 v3 se, use button or arrow to navigate to next page (should be on 2nd page)
4. Click on the printer
5. Wait for it to connect. P.S. if it does not connect, make sure to recheck the steps you did on [Installing motherboard firmware](#installing-motherboard-firmware)
6. If connection was successfully, it will start doing some stuff. Let it do its thing, be patient! If this fails make sure to check out the fixes [TODO Link] if you encounter errors.
7. Click **OK**
8. Now you can follow the [Rooting guide](../rooting/index.md).
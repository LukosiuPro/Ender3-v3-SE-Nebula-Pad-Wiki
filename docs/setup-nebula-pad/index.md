# Setting up the Nebula Pad

!!! important
    Creality print right now does not have motherboard firmware files, so these are my local ones that I have, when they fix their site, I will update this to their links. USE AT YOUR OWN RISK!
    
    * The newer "C14" mainboard only work with these firmware files: [Ender3 v3 SE C14 motherboard firmware files](../../files/Ender3V3Se_stm32f401_klipper下位机.rar). Thanks to @absk1s3 for the files.
    
    * For C13 motherboard please use the older files from here: [Ender3 v3 SE C13 motherboard firmware files](../../files/3d-print-firmware.zip) Alternatively for C13 motherboard you can use the wayback machine to get those from [old site](https://web.archive.org/web/20250731114403/https://www.creality.com/pages/download-creality-nebula-smart-kit).

!!! info
    Some of the instructions here reference files you can download from the [Creality Downloads](https://www.creality.com/pages/download-creality-nebula-smart-kit) page for the Nebula Pad. These files are also included on the USB drive that comes with the Nebula Kit. You can use those files if you wish, but they may be outdated. When working on the setup, it is recommended to use the freshly downloaded versions. 

Before you can do a lot of cool stuff with the Nebula Pad, you need to install it first. While the official manual offers some help, it is not specific to the Ender-3 V3 SE, which can lead to odd errors.

Before installing the kit, you may want to print a bracket for the new Nebula Pad as it will not fit on the stock bracket. There is a bracket model at the downloads page. If you want something simpler, you can also print an [adapter](https://www.thingiverse.com/thing:6371800) that lets you mount the Pad on the stock bracket.

## Install Motherboard Firmware

The default firmware for the Ender-3 V3 SE is designed to work with the stock screen. The Nebula Pad will not connect to the printer until you update the printer's motherboard to firmware that works with the Nebula Pad.

!!! tip inline end
    You will need to use an SD card to update the printer's firmware. An improperly formatted card can cause failures in the update process. Make sure that the SD card is [correctly formatted](../general/format-sd.md) before beginning.

1. Make sure the printer is powered off.
2. Unplug the old screen.
3. Download the "3D Print Firmware" from the downloads page.
4. Extract the contents of the downloaded archive.
5. Put the printer's SD card into your computer and copy the file `Ender3V3SE_firmware.bin`, or take the `firmware.bin` file, if you use a C14 files, to the root of the card.
6. Rename the file to `firmware.bin`.
7. Put the card into the printer and turn it on.
8. Wait **at least 5 minutes** and then turn off the printer.
9. Remove the SD card from the printer.
10. Connect the Nebula Pad to the printer.
11. Make sure that there is no USB cable connected to either the Nebula Pad or the printer and that the SD Card slot is empty.
12. Turn on the printer. If the update was successful, the Nebula Pad will begin the setup process and prompt for the language you wish to use.

At this point, you can proceed to [setup the Nebula Pad](#setup-the-nebula-pad).

## Setup the Nebula Pad

1. When you boot up for the first time, you will be greeted with a printer selection dialog.
2. Depending on the firmware version on your Nebula Pad, you will see either arrows or page buttons to go between pages in the list.
3. Find the "Ender-3 V3 SE" in the list. This will usually be on the second or third page.
4. Tap on the listing.
5. The Nebula Pad will now try to connect and communicate with the printer. If it does not connect, make sure you [installed the motherboard firmware](#install-motherboard-firmware) before setting up the pad.
6. Once the connection is successful, the Pad will start running some tests and calibrations including z-level offset and bed mesh probing. This can take a while, so be patient.
7. Once the test and calibrations are complete, you are ready to [root the pad](../rooting/index.md).

# Rooting the Nebula Pad

Once you have installed the Nebula Pad on your printer, you can "root" it. This lets you make tweaks and enable extra features that are not available in the default firmware.

!!! danger "At Your Own Risk"
    3D FDM printers involve high temperatures, molten plastic, and electricity. Improperly done modifications may not only break your printer but may cause damage, personal harm, or death. Any modifications you make are at your own risk. Please make sure to follow all [safety](../safety.md) notes and your own common sense when working on your printer.

## Confirming Version 1.1.0.29

This document covers installing a "rooted" version of the Nebula Pad firmware version 1.1.0.29. If your pad is running
an older version, you will want to upgrade first to ensure a clean setup. It is also recommended that you do not set up
a wireless network connection on the stock firmware.

1. Open [creality website](https://www.creality.com/pages/download-creality-nebula-smart-kit),
2. Under "**Download Product Firmware**" section find `NEBULA_ota_img_V1.1.0.29.img` and click download.
3. Now find your usb drive that came with nebula pad.
4. Make sure there is **no firmware file already on it** that ends with `.img`. If you have remove the file.
5. (Optional) clear the flash drive from other files. 
6. Put the downloaded file onto USB drive.
7. Use eject function on your pc and unplug the usb drive.
8. **Make sure you are not connected to the internet** and then plug the usb drive into nebula pad.
9. Nebula pad should pick up the update file and will prompt you for update. 
10. Click update.

## Installing Rooted Firmware

!!! important
    Before following the below steps, make sure your Nebula Pad is running the official firmware version 1.1.0.29. If it
    is not, follow the steps in the previous section before proceeding.

Before starting this process, it is recommended that you do a factory reset on the Pad. You can do a reset by going to
the gear section on the Pad, then scroll to the bottom on the System tab to find the option.

1. Download firmware from [here](https://mega.nz/file/Kox1kYCJ#6QWxVtRq9qEWKdZIfl0-O0lnbYkpP1nnKZtUjiZ8J80).
2. Grab usb drive that came with nebula pad. 
3. Make sure there is **no firmware file already on it** that ends with `.img`. If you have remove the file. 
4. (optional) remove any other file that is on the usb drive, to reduce likely chance of failure.
5. Copy the downloaded file to usb drive. 
6. Unmount the drive from your pc.
7. Unplug the USB drive.
8. Plug it into the nebula pad.
9. Give it a moment and you should see an update with version number `V6.1.0.29`
10. Click update.
11. Wait for it to finish and after restart, unplug the drive.

## Installing Mainsail and Fluidd

If the rooted firmware install was successful, you can now install Mainsail and Fluidd to get a remote interface for
your printer that will also let you print directly from some slicer software.

1. If you did a factory reset before installing, you will be walked through the Pad setup. You can connect to a network,
   but it is recommended you not connect to the Creality Cloud.
2. Once the printer is connected to the network and ready, you can try [SSH'ing into the nebula pad](../general/nebula-pad-ssh.md).
   When you open ssh session type:
    ```Bash
    ./installer.sh
    ```
   This will download and then launch the helper script.
3. At the main menu, choose the option to install.
4. At the next menu, install "Moonraker and Nginx" and "Fluidd" from the essentials section at minimum.
5. When the install is done, quit the script and then run "reboot" to restart the Nebula Pad and the newly installed tools.
6. Once the Pad has started back up, you can open a web browser and access the Fluidd interface by browsing to `http://your-printer:4408/`. If you're not sure of the IP, you can [follow this guide to find it](../general/find-ip.md).

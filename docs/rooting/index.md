# Rooting the Nebula Pad

Once you have installed the Nebula Pad on your printer, you can "root" it. This lets you make tweaks and enable extra features that are not available in the default firmware.

!!! danger "At Your Own Risk"
    3D FDM printers involve high temperatures, molten plastic, and electricity. Improperly done modifications may not only break your printer but may cause damage, personal harm, or death. Any modifications you make are at your own risk. Please make sure to follow all [safety](../safety.md) notes and your own common sense when working on your printer.

## Downgrading to Version 1.1.0.23

This document covers installing a "rooted" version of the Nebula Pad firmware version 1.1.0.23. If your pad is running a newer version, you will need to downgrade first or the process could cause problems with your printer.

1. Open [creality website](https://www.creality.com/pages/download-creality-nebula-smart-kit),
2. Under "**Download Product Firmware**" section find `NEBULA_ota_img_V1.1.0.23.img` and click download.
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
    Before following the below steps, make sure your Nebula Pad is running the official firmware version 1.1.0.23. If it is not, follow the steps in the previous section before proceeding.

1. Download firmware from [here](https://www.openk1.org/cfw/NEBULA-destinal-cfw-0.5-ota_img_V5.1.0.23.img).
2. Grab usb drive that came with nebula pad. 
3. Make sure there is **no firmware file already on it** that ends with `.img`. If you have remove the file. 
4. (optional) remove any other file that is on the usb drive, to reduce likely chance of failure.
5. Copy the downloaded file to usb drive. 
6. Unmount the drive from your pc.
7. Unplug the USB drive.
8. Plug it into the nebula pad.
9. Give it a moment and you should see an update with version number `V5.1.0.23`
10. Click update.
11. Wait for it to finish and after restart, unplug the drive.
12. If the root was successfully, you can try [SSH'ing  into the nebula pad](../general/nebula-pad-ssh.md).
13. When you open ssh session type:
    ```Bash
    ./installer.sh
    ```
14. In the installer, type `5` and click enter
15. Make sure the first 3 is installed (`Moonraker`, `Fluidd` and `Mainsail`).
16. If one of them is not installed, follow updating the helper script [TODO Link] and fixing core programs install [TODO Link]
else continue onward.
17. Open your browser and type `YOUR_PRINTER_IP:4408`. If you don't know how to get the ip of nebula pad follow [this](../general/find-ip.md).
18. If you can't get the page to open, it can be one of many things:
    - Your router does not allow local communication with the printer. [TODO How to fix]
    - You are not on the same network as your printer. [TODO How to fix]
    - Corrupted `Moonraker`/`Fluid` install [TODO How to fix]
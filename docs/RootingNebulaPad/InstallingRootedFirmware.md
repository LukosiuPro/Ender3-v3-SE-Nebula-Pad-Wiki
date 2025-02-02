# Installing rooted firmware

**IMPORTANT!!!** Before following, make sure you are on version 23 firmware! How to downgrade you can find [here](./DowngradingNebulaPad.md)

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
12. If the root was successfully, you can try [SSH'ing  into the nebula pad](../GeneralTutorials/SSHIntoNebulaPad.md).
13. When you open ssh session type:
    ```Bash
    ./installer.sh
    ```
14. In the installer, type `5` and click enter
15. Make sure the first 3 is installed (`Moonraker`, `Fluidd` and `Mainsail`).
16. If one of them is not installed, follow updating the helper script [TODO Link] and fixing core programs install [TODO Link]
else continue onward.
17. Open your browser and type `YOUR_PRINTER_IP:4408`. If you don't know how to get the ip of nebula pad follow [this](../GeneralTutorials/GettingPrinterIp.md#getting-printer-ip).
18. If you can't get the page to open, it can be one of many things:
    - Your router does not allow local communication with the printer. [TODO How to fix]
    - You are not on the same network as your printer. [TODO How to fix]
    - Corrupted `Moonraker`/`Fluid` install [TODO How to fix]
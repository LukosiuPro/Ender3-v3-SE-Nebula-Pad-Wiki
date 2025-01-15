# SSH'ing into the nebula pad

Note: You can only ssh into the nebula pad successfully, if you have it rooted.

## Windows
- Recommended software to use [mobaXtream](https://mobaxterm.mobatek.net/download.html)

1. Open mobaXterm.
2. Click on Session in toolbar at top left.
3. Click on SSH
4. Enter Ip Of your printer. [TODO how to find the ip]
5. Leave everything else as is and click OK.
6. It will open the terminal windows asking for username, if it doesn't, follow troubleshooting guide. [TODO guide]
7. For username enter`root` and click enter.
8. For password enter `creality` and click enter. 
9. Now you should see the left side window populate with files and the terminal show `$` sign next to `root`.

## Linux/MAC
- Recommended software putty or terminal

1. Open terminal
2. Type 
    ```BASH
   ssh root@YOUR_PRINTER_IP
   ```
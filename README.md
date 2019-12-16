# linux-boot-on-eemc-disk
How to boot elementary OS on Lenovo ideapad with eemc disk


I purchased new a Lenovo Ideapad 110s sold with pre-installed Windows 10. After finding the Windows 10 and Lenovo software took about 27 Gb of the 32 Gb SSD, and "important" Windows 10 updates wouldn't download owing to lack of disk space, obviously the unit was only set up for people short on ideas and no wish to update.
So dumping Windows 10 altogether I installed Linux Mint 19 Xfce from an external USB-connected DVD drive. Installation seemed smooth, but the Ideapad wouldn't reboot.
After some digging on this and Ubuntu forums I've just successfully reinstalled the Xfce with the following settings in BIOS:
   
    CONFIGURATION:
    USB Legacy - Enabled
    Wireless - Enabled
    Hotkey Mode - Not relevant
    Intel Virtual Technology - Enabled
    BIOS Flash Back - Disabled
    
    SECURITY:
    Intel Trust Platform Technology - Disabled
    
    BOOT:
    Boot Mode - Legacy Support
    Boot Priority - UEFI First
    USB Boot - Enabled
    PXE Boot To LAN - Disabled
    
    EXIT:
    OS Optimized Defaults - Disabled

I installed this time without using the wi-fi (to speed up installation). Rebooting worked fine, I've now connected the wi-fi and downloaded updates. Less than 30% of the SSD is used by the current setup.

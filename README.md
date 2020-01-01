# Windows 10 Tools

Unfortunately, I am still required to use windows for certain tasks, such as NTFS drives, optical media, some games, my scanner, and family and friends tech support.  I am still using Windows 7 as my only Windows machine, but I fear that the time will soon be upon us when Windows 7 is no longer viable, as was ultimately the case with Windows XP.

These are the things I use to make my life a little easier when I am forced to deal with Windows 10.


## New Installation Checklist

* Run `stop_installing_games.reg` IMMEDIATELY
* Right Click Taskbar -> Taskbar settings -> Select which icons appear on the taskbar -> Always show all
* Install this stuff:
    * Chrome (Firefox installations always fail for 64 bit!)
    * 7zip
    * Comodo Firewall (`cfw_installer_5.3.181415.1237_64.msi`)
        * Uncheck "Install COMODO Antivirus"
        * Choose "Firewall Only"
        * Choose "I do not want to use COMODO SecureDNS Servers"
        * reboot
        * Firewall Security Level -> Custom Policy
        * Turn off auto update
        * Change appearance to `Windows Theme`
    * ImgBurn
    * ScanSnap
* Explorer -> View -> File Name Extensions
* Control Panel -> Programs and Features -> Windows Features
    * .net 3.5
    * Windows subsystem for Linux
    * reboot
* Settings -> Update & Security
    * check for updates, which will install themselves automatically
    * reboot


## stop_installing_games.reg

I can't believe that in 2019, I have to deal with Microsoft installing things like Candy Crush and Facebook to my operating system that cost hundreds of dollars.  Thankfully, there's an easy way to get it to stop.

Download the `.reg` file, then double click on it.  Boom.

Credit: [https://winaero.com/blog/fix-windows-10-installs-apps-like-candy-crush-soda-saga-automatically/](https://winaero.com/blog/fix-windows-10-installs-apps-like-candy-crush-soda-saga-automatically/)


## Fixing boot

When Windows won't boot, even after you've tried the various boot options in the bios, you can try this:

1. Insert the Windows 10 installation USB
1. Press the `delete` key a bunch of times until the bios options come up
1. Choose the `UEFI` boot option that corresponds to the USB drive
1. Click `Next` on the language option menu
1. Click `Repair Your Computer` near the bottom left
1. Click `Troubleshoot`
1. Click the `Command Prompt` option
1. Run the command `diskpart`
1. Find the disk you want to fix
    1. `list disk`
    1. For me, it was `disk 0`
1. Make a note of the Volume Letter
    1. For me, it was `C`
1. `exit`
1. `cd /d C:`
1. `bootrec /fixmbr`
1. `bootrec /fixboot`
1. `bootrec /rebuildbcd`


## References

* https://www.dell.com/support/article/us/en/04/sln300987/how-to-repair-the-efi-bootloader-on-a-gpt-hdd-for-windows-7-8-8-1-and-10-on-your-dell-pc?lang=en
* https://www.easeus.com/partition-manager-software/fix-uefi-boot-in-windows-10-8-7.html

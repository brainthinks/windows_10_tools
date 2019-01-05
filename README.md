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

# Windows 10 Tools

Unfortunately, I am still required to use windows for certain tasks, such as NTFS drives, optical media, some games, my scanner, and family and friends tech support.  I am still using Windows 7 as my only Windows machine, but I fear that the time will soon be upon us when Windows 7 is no longer viable, as was ultimately the case with Windows XP.

These are the things I use to make my life a little easier when I am forced to deal with Windows 10.


## New Installation Checklist

* LEAVE THE ETHERNET CABLE UNPLUGGED AND WIFI DISCONNECTED!! NO NETWORKING!!
* Run `stop_installing_games.reg` IMMEDIATELY
* Right Click Taskbar -> Taskbar settings
    * Taskbar location -> left
    * Select which icons appear on the taskbar -> Always show all
    * Combine Taskbar buttons -> Never
    * Show taskbar on all displays -> off
    * Search for theme
    * Themes and Related Settings -> Colors -> Dark mode
* Explorer -> View -> File Name Extensions
* Install Netlimiter Firewall
    * Turn off the limiter
    * Turn off priorities
    * Tools -> Options
        * Service -> Blocker
            * Default Blocker Action In -> Ask
            * Default Blocker Action Out -> Ask
        * Client -> Theme
            * Base Color -> Dark Gray
        * Client -> Tray Icon
            * Select all
* Plug in ethernet cable or connect to wifi
* Do all windows updates, restart, repeat until up to date
* Install this stuff:
    * 7zip
    * Brave Browser (Firefox installations always fail for 64 bit!)
    * Everything search
    * vlc
    * vscode
* Control Panel -> Programs and Features -> Windows Features
    * .net 3.5
    * Windows subsystem for Linux
    * reboot


## stop_installing_games.reg

I can't believe that in 2019, I have to deal with Microsoft installing things like Candy Crush and Facebook to my operating system that cost hundreds of dollars.  Thankfully, there's an easy way to get it to stop.

Download the `.reg` file, then double click on it.  Boom.

Credit: [https://winaero.com/blog/fix-windows-10-installs-apps-like-candy-crush-soda-saga-automatically/](https://winaero.com/blog/fix-windows-10-installs-apps-like-candy-crush-soda-saga-automatically/)

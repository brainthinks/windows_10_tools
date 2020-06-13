# Windows 10 Tools <!-- omit in toc -->

Unfortunately, I am still required to use windows for certain tasks, such as NTFS drives, optical media, some games, my scanner, and family and friends tech support.  I am still using Windows 7 as my only Windows machine, but I fear that the time will soon be upon us when Windows 7 is no longer viable, as was ultimately the case with Windows XP.

These are the things I use to make my life a little easier when I am forced to deal with Windows 10.


## Table of Contents <!-- omit in toc -->

- [New Installation Checklist](#new-installation-checklist)
- [stop_installing_games.reg](#stopinstallinggamesreg)
- [Outlook](#outlook)
  - [Transfer Autocomplete Entries](#transfer-autocomplete-entries)


## New Installation Checklist

* LEAVE THE ETHERNET CABLE UNPLUGGED AND WIFI DISCONNECTED!! NO NETWORKING!!
* Run `stop_installing_games.reg` IMMEDIATELY
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
* Right Click Desktop -> Personalize
    * Colors
        * Choose your color -> Dark
        * Show accent color on the following surfaces -> check all
    * Lock Screen
        * Background -> Picture
        * Get fun facts -> Off
    * Start
        * Turn ALL Off
        * Choose which folders appear on Start
            * File Explorer
            * Settings
            * Downloads
            * Network
            * Personal Folder
    * Taskbar
        * Taskbar location -> left
        * Select which icons appear on the taskbar -> Always show all
        * Combine Taskbar buttons -> Never
        * Show taskbar on all displays -> off
* Unpin everything except Explorer Folder from taskbar
* Right click on all start menu tiles and remove them
* Explorer -> View -> File Name Extensions
* set default applications
    * Music -> VLC
    * Videos -> VLC
    * Web browser -> Firefox
* Install this stuff:
    * dropbox?
        * re-link personal folders from my pc?
    * 7zip
    * Browsers
        * New Chromium-based Edge
        * Firefox
        * Brave Browser
        * Chrome, if you must
    * Install `ublock origin` in all browsers
    * Everything - [https://www.voidtools.com/](https://www.voidtools.com/)
    * vlc
    * vscode
    * cobian backup - [https://www.cobiansoft.com/](https://www.cobiansoft.com/)
    * KeePassX - [https://www.keepassx.org/](https://www.keepassx.org/)
    * printer drivers?
    * adobe acrobat reader
    * teamviewer
* Control Panel -> Programs and Features -> Windows Features
    * .net 3.5
    * Windows subsystem for Linux
    * reboot


## stop_installing_games.reg

I can't believe that in 2019, I have to deal with Microsoft installing things like Candy Crush and Facebook to my operating system that cost hundreds of dollars.  Thankfully, there's an easy way to get it to stop.

Download the `.reg` file, then double click on it.  Boom.

Credit: [https://winaero.com/blog/fix-windows-10-installs-apps-like-candy-crush-soda-saga-automatically/](https://winaero.com/blog/fix-windows-10-installs-apps-like-candy-crush-soda-saga-automatically/)


## Outlook

### Transfer Autocomplete Entries

* [https://support.office.com/en-us/article/import-or-copy-the-auto-complete-list-to-another-computer-83558574-20dc-4c94-a531-25a42ec8e8f0](https://support.office.com/en-us/article/import-or-copy-the-auto-complete-list-to-another-computer-83558574-20dc-4c94-a531-25a42ec8e8f0)
* [https://stephenegriffin.github.io/mfcmapi/](https://stephenegriffin.github.io/mfcmapi/)

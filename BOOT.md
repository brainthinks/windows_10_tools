# Windows Boot

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
1. Find the volume you want to make bootable
    1. `sel disk 0`
    1. `list vol`
    1. Make a note of the Volume Letter
        1. For me, it was `C`
1. `exit`
1. `cd /d C:`
1. `bootrec /fixmbr`
1. `bootrec /fixboot`
1. `bootrec /rebuildbcd`
    1. You may be prompted to select a Windows location
    1. For me, this time, it was Windows.old
    1. I didn't like that option, so I selected no, but no other options were available
    1. I reran `bootrec /rebuildbcd` and selected the option it gave me by entering `Y` and pressing `Enter`
1. `exit`
1. Select `Turn Off Your PC`
1. Turn your computer back on - hopefully it boots

Note that I had to do this when I applied the latest Windows update (2020-01-18).  When mine rebooted the second time, I was prompted with a screen to select my operating system... pathetic, Microsoft.


## References

* https://www.dell.com/support/article/us/en/04/sln300987/how-to-repair-the-efi-bootloader-on-a-gpt-hdd-for-windows-7-8-8-1-and-10-on-your-dell-pc?lang=en
* https://www.easeus.com/partition-manager-software/fix-uefi-boot-in-windows-10-8-7.html

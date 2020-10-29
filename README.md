# Installer_Dell-Inspiron-5570_Catalina
USB installer image for MacOS Catalina for a Dell Inspiron 5570


## Before you Install

- Download this: https://github.com/stayboogy/Hackintosh_Dell-Inspiron-5570_Catalina.git  extract, and put the files on another usb drive formatted fat32, this is very important

## How to Install
For Advanced Users ONLY

- First you will have to combine these individual pieces into one .img.  This can be done using "cat DellInspiron5570_Catalina_Installer.img.* > DellInspiron5570_Catalina_Installer.img" In Windows you can use 7z.
- Make sure SATA is set to AHCI in BIOS--go back to RAID after install and successful reboots.
- Apply this image to a USB flash drive of any size larger than 8GB.
- You can do this in Windows by using Win32 Disk Imager, or in Linux and MacOS using dd.  
- Make sure boot options in BIOS are set to UEFI
- There is a chance you may have to boot to BIOS with the usb in the slot and add the usb as a uefi boot path in the bios with /EFI/CLOVER/CLOVERX64.EFI as the boot path.  This is under boot configuration.  If you don't know what this is or how to add an boot option to your uefi setup, then don't attempt any of this.
- Boot from this usb and install just like you would any other OS--I suggest that you clean install this and format your entire disk and then re-install Windows after.  It's much easier this way and ensures that the proper EFI from my other repo works properly.
- DO NOT REBOOT after MacOS loads--open the clover app from the POST_INSTALL folder on your other fat32 usb.  Mount your EFI partition.  Open it in Finder and delete your EFI folder completely, and then copy over the EFI folder from your other fat32 usb.
- Remove the usb and reboot.

You should now have MacOS Catalina running on your 5570 like it built for it.



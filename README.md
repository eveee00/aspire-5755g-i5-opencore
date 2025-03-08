# aspire-5755g-i5-opencore
WIP OpenCore files for the Acer Aspire 5755G i5 variant.

## Disclaimer
**DO NOT USE THIS IN A PRODUCTION ENVIRONMENT! THE LATEST MACOS THAT SUPPORTS THIS LAPTOP IS MACOS 10.13 HIGH SIERRA! THIS RELEASE IS *8 YEARS OLD* AND DOESN'T RECEIVE SECURITY PATCHES ANYMORE!**
### I CLAIM *ABSOLUTELY NO* RESPONSIBILITY IF YOU FUCK SOMETHING UP! *YOU* ARE CHOOSING TO INSTALL OUT-OF-DATE SOFTWARE ONTO *YOUR* DEVICE!

If you want something modern for this laptop, consider going with [Linux Mint](https://www.linuxmint.com/) or [Fedora](https://fedoraproject.org/) (I recommend the [KDE Spin](https://fedoraproject.org/spins/kde)).

## What DIDN'T Work
- Sound (ALCID 2, Microphone untested since my laptop's mic is broken)

## What DOESN'T work:
- WiFi (Broadcom Chip)
- ~~CPU Power optimizations~~ Dummy Power Management has to be set to true to avoid a kernel panic
- ~~Brightness Keys~~ (FN + F12 to decrease, FN + Pause to increase. On USB Keyboards it's Scroll lock to decrease and Pause to increase)
- eGPU (Will never work unless someone successfully dumps the vBIOS)
- USB 3
- Mouse and Keyboard in the boot picker
- Battery Info (Tried with both ECEnabler and SMCBatteryManager)

## Screenshot

![screen2](https://github.com/user-attachments/assets/34db68bb-d78f-4279-81d1-fc703b361d2a)

## Extra Info

Guide to create the USB: https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html

Follow step 3 of [this guide](https://mrmacintosh.com/how-to-fix-the-recovery-server-could-not-be-contacted-error-high-sierra-recovery-is-still-online-but-broken/) if you get an error about a server connection in recovery.

You need to follow the [diskpart + legacy install method](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#diskpart-method) to boot this. You need to use a USB keyboard to navigate the boot menu or you can wait for the timeout and it auto-selecting the USB.

Note: I was able to boot MacOS 15, but ethernet refuses to work. I'll maybe try to get the WiFi card up and running or try to create an offline installer.

## Attributions
are in [attribution.md](https://github.com/eveee00/aspire-5755g-i5-opencore/blob/main/attribution.md)

## Old README
~~**As of now (04.03.2025 - 02:50) this config fails to boot on my laptop. Something about a non-bootable floppy. I'll work on this sometime in the future**~~

UPDATE: It boots now! (only through USB2.0). I'll upload a new release ~~after I get the keyboard and the recovery working.~~

# aspire-5755g-i5-opencore
WIP OpenCore files for the Acer Aspire 5755G i5 variant.

## Disclaimer
**DO NOT USE THIS IN A PRODUCTION ENVIRONMENT! THE LATEST MACOS THAT SUPPORTS THIS LAPTOP IS MACOS 10.13 HIGH SIERRA! THIS RELEASE IS *8 YEARS OLD* AND DOESN'T RECEIVE SECURITY PATCHES ANYMORE!**
### I CLAIM *ABSOLUTELY NO* RESPONSIBILITY IF YOU FUCK SOMETHING UP! *YOU* ARE CHOOSING TO INSTALL OUT-OF-DATE SOFTWARE ONTO *YOUR* DEVICE!

If you want something modern for this laptop, consider going with [Linux Mint](https://www.linuxmint.com/) or [Fedora](https://fedoraproject.org/) (I recommend the [KDE Spin](https://fedoraproject.org/spins/kde)).

## What DOESN'T work:
- Sound
- WiFi (Broadcom Chip)
- CPU Power optimisations
- Brightness Keys
- eGPU
- USB 3

## Screenshot

![screen](https://github.com/user-attachments/assets/849bef32-b11c-407b-ba58-8eee5484c2ee)

## Extra Info

Guide to create the USB: https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html

Follow step 3 of [this guide](https://mrmacintosh.com/how-to-fix-the-recovery-server-could-not-be-contacted-error-high-sierra-recovery-is-still-online-but-broken/) if you get an error about a server connection in recovery.

You need to follow the [diskpart + legacy install method](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#diskpart-method) to boot this. You need to use a USB keyboard to navigate the boot menu or you can wait for the timeout and it auto-selecting the USB.

## Attributions
are in [attribution.md](https://github.com/eveee00/aspire-5755g-i5-opencore/blob/main/attribution.md)

## Old README
~~**As of now (04.03.2025 - 02:50) this config fails to boot on my laptop. Something about a non-bootable floppy. I'll work on this sometime in the future**~~

UPDATE: It boots now! (only through USB2.0). I'll upload a new release ~~after I get the keyboard and the recovery working.~~

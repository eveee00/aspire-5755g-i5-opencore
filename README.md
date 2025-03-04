# aspire-5755g-i5-opencore
WIP OpenCore files for the Acer Aspire 5755G i5 variant.
~~**As of now (04.03.2025 - 02:50) this config fails to boot on my laptop. Something about a non-bootable floppy. I'll work on this sometime in the future**~~

UPDATE: It boots now! (only through USB2.0). I'll upload a new release ~~after I get the keyboard and the recovery working.~~

You need to follow the [diskpart + legacy install method](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#diskpart-method) to boot this. You need to use a USB keyboard and MacOS currently throws a kernel panic. OpenCore also refuses to load the SSDTs. (most likely cause of the panic). 

This is the current OC log, if anyone is interested:
```
00:000 00:000 OC: Failed to drop ACPI 54445353 0000006D50757043 0 (1) - Not Found
00:066 00:066 OC: Failed to drop ACPI 54445353 0074734930757043 0 (1) - Not Found
00:181 00:115 OCA: Inserted ACPI table has length mismatch 229429 vs 557582858, ignoring
00:248 00:066 OC: Failed to add ACPI SSDT-EC-LAPTOP.aml - Invalid Parameter
00:365 00:117 OCA: Inserted ACPI table has length mismatch 229540 vs 557582858, ignoring
00:432 00:066 OC: Failed to add ACPI SSDT-PNLF.aml - Invalid Parameter
00:534 00:101 OCA: Inserted ACPI table has length mismatch 229263 vs 557582858, ignoring
00:601 00:066 OC: Failed to add ACPI SSDT-XOSI.aml - Invalid Parameter
```

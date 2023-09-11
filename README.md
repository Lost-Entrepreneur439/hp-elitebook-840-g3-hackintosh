# hp-elitebook-840-g3-hackintosh-ventura
A prebuilt Opencore EFI for macOS Ventura on the HP Elitebook 840 G3

This is a macOS Ventura EFI for the HP Elitebook 840 G3, with support for Intel Wi-Fi cards. 13.5.2 working, with OpenCore 0.9.5 and fully up to date kexts. Remember to keep your kexts and OpenCore up to date! Remember to change your SMBIOS data too.

![Screenshot](https://github.com/Lost-Entrepreneur439/hp-elitebook-840-g3-hackintosh-ventura/blob/main/Untitled%202.png)

# Specs of my specific unit:
* CPU: Intel Core i5-6300U
* GPU: Intel HD Graphics 520
* Touchpad: Synaptics SMBus
* Audio - Conexant CX20724
* Wi-Fi/Bluetooth - Intel Wireless-AC 8260
* Ethernet - Intel I219-LM
* SSD - Micron 256GB mSATA

Follow the "Downloading macOS" section in the Dortania guide to get macOS - https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#downloading-macos

## Set bios settings as follows:
* Security -> Intel Software Guard Extensions (SGX) -> Disable

* Advanced -> Boot Options -> Uncheck “Fast Boot”

* Advanced -> Boot Options -> Check “UEFI Boot Order”

* Advanced -> Boot Options -> Uncheck “Legacy Boot Order”

* Advanced -> Secure Boot Configuration -> Configure Legacy Support and Secure Boot -> Legacy Support Disable and Secure Boot Disable

* Advanced -> System Options ->  Check “Hyperthreading”

* Advanced -> System Options -> Check “Virtualization Technology (VTx)”

* Advanced -> System Options -> Uncheck “Virtualization Technology for Directed I/O (VTd)”

* Advanced -> Built-In Device Options -> Video memory size -> 64MB or anything higher

# Credits

[Dortania](https://github.com/dortania) -- Made the OpenCore guide which was used to create this EFI

[Acidanthera](https://github.com/acidanthera) -- Made OpenCore, AppleALC, BlueToolFixup, BrightnessKeys, IntelMausi, Lilu, SMCBatteryManager, SMCProcessor, VirtualSMC, VoodooPS2Controller & WhateverGreen

[OpenIntelWireless](https://github.com/OpenIntelWireless) -- Made airportitlwm & IntelBluetoothFirmware

[Avery Black](https://github.com/1Revenger1) -- Made ECEnabler

[钟先耀](https://github.com/zxystd) -- Made IntelBTPatcher

[FireWolf](https://github.com/0xFireWolf) -- Made RealtekCardReader

[USBToolBox](https://github.com/USBToolBox) -- Made USBToolBox & UTBMap

[VoodooSMBus](https://github.com/VoodooSMBus) -- Made VoodooRMI & VoodooSMBus

[CorpNewt](https://github.com/corpnewt) -- Helped me fix external display issues

[HP](https://www.hp.com/us-en/home.html) -- Made the EliteBook 840 G3

[Apple](https://www.apple.com/ca/) -- Made macOS

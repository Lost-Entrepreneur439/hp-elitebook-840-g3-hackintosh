# hp-elitebook-840-g3-hackintosh-ventura
A prebuilt Opencore EFI for macOS Ventura on the HP Elitebook 840 G3

**WARNING! Ethernet IS required for initial half of setup if you use an internet-based installer. You will need to install Heliport for Wi-Fi.**

This is a macOS Ventura EFI for the HP Elitebook 840 G3, with support for Intel Wi-Fi cards. 13.3.1a working, with OpenCore 0.9.1 and fully up to date kexts. Remember to keep your kexts and OpenCore up to date! I recommend OCAuxiliaryTools to keep your kexts and OpenCore up to date. Remember to change your SMBIOS data too.

![Screenshot](https://github.com/Lost-Entrepreneur439/hp-elitebook-840-g3-hackintosh-ventura/blob/main/Untitled%202.png)

# Specs of my specific unit:
* CPU: Intel Core i5-6300U
* GPU: Intel HD Graphics 520
* Resolution: 1920x1080
* Audio: Intel Sunrise Point-LP PCH
* Wi-Fi+Bluetooth: Intel AC-8260
* Ethernet: Intel I219-LM
* Touchpad: Synaptics

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

[Dortania](https://github.com/dortania) -- Made the OpenCore guide which was used to create this EFI and CtlnaAHCIPort

[Acidanthera](https://github.com/acidanthera) -- Made Opencore, AppleALC, BlueToolFixup, IntelMausi, Lilu, RTCMemoryFixup, VirtualSMC, VoodooInput, VoodooPS2Controller and WhateverGreen

[OpenIntelWireless](https://github.com/OpenIntelWireless) -- made IntelBluetoothFirmware and itlwm

[zxystd](https://github.com/zxystd) -- Made IntelBTPatcher

[cholonam](https://github.com/cholonam) -- Made Sinetek-rtsx

[corpnewt](https://github.com/corpnewt) -- Made USBMap

[VoodooSMBus](https://github.com/VoodooSMBus) -- Made VoodooRMI and VoodooSMBus

[1Revenger1](https://github.com/1Revenger1) -- Helped me fix trackpoint and top mouse buttons

[Apple](https://www.apple.com/ca/) -- Made macOS

[HP](https://www.hp.com/ca-en/home.html) -- Made the Elitebok 840 G3

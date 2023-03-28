# hp-elitebook-840-g3-hackintosh-ventura
A prebuilt Opencore EFI for macOS Ventura on the HP Elitebook 840 G3

This is a macOS Ventura EFI for the HP Elitebook 840 G3, with support for Intel Wi-Fi cards. 13.3 working, with OpenCore 0.9.0 and fully up to date kexts. Remember to keep your kexts and OpenCore up to date! I recommend OCAuxiliaryTools to keep your kexts and OpenCore up to date. Remember to change your SMBIOS data too.

![Screenshot](https://github.com/Lost-Entrepreneur439/hp-elitebook-840-g3-hackintosh-ventura/blob/main/Untitled%202.png)

# Specs of my specific unit:
* CPU: Intel Core i5-6300U
* GPU: Intel HD Graphics 520
* Resolution: 1920x1080
* Audio: Intel Sunrise Point-LP PCH
* Wi-Fi+Bluetooth: Intel AC-8260
* Ethernet: Intel I219-LM
* Touchpad: Synaptics

## Set bios settings as follows:
Advanced tab:  
Boot options:  
- Fast Boot = Disabled
- Network (PXE) Boot = Disabled  
Secure Boot Configuration:
- "Legacy Support Disable and Secure Boot Disable"  (Legacy can be enabled if needed, however do not turn on Secure Boot.)
System Options:  
- Virtualization Technology (VTx) = Enabled
- Virtualization Technology for Direct I/O (VTd) = Disabled  
Built-In Device Options:  
- Wake On LAN = Disabled
- Video memory size = 64MB or higher
- LAN/WLAN Auto Switching = Disabled
- Fingerprint Device = Disabled  
Power Management Options:  
- Extended Idle Power States = Disabled
- Deep sleep = You can keep this enabled
- Wake when Lid is Opened = Enabled
- Wake on USB = Disabled

## Problems
* Dualbooting with Windows 7 and Windows 8.1 not working. Windows 10 and 11 dualboot is untested. Use the F9 boot menu or rEFInd for dualbooting with 7 or 8.1 (discovered by me)
* Graphical glitches when scrolling in Safari on some units (discovered by u/UpstairsAd6594 on Reddit)
* If the laptop's battery dies when in sleep mode, when the laptop turns back on, macOS will act like the laptop is rebooting from a kernel panic, displaying the "Your computer rebooted because of a problem" message. (Discovered by me)
* You tell me!

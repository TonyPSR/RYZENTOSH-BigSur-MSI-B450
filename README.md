# RYZENTOSH-BigSur-MSI-B450

## Specs

| Component           | Detail                                              |
| ------------------- | --------------------------------------------------- |
| Processor           | Ryzen 7 2700 8C/16T (non-X)                         |
| Motherboard         | MSI B450 TOMAHAWK MAX                               |
| Memory              | 16GB(8x2) Crucial Ballistix DDR4 3000 MHz           |
| SSD                 | Crucial BX500 120GB                                 |
| iGPU                | None                                                |
| Graphics Card       | GIGABYTE NVIDIA GeForce GT710 2GB DDR3              |
| Monitor             | HP 24es 1080p IPS (24inch)                          |
| Sound Card          | Realtek ALC892 Codec                                |
| LAN                 | Realtek® 8111H Gigabit LAN controller               |

> OpenCore Verison: 0.6.5

> MacOS supported: macOS 11 Big Sur

## macOS 10.15.x Catalina build: https://github.com/TonyPSR/RYZENTOSH-Catalina-MSI-B450

# Don't forget to update MLB, SystemSerialNumber and SystemUUID under PlatformInfo key in config.plist!!!
#### For macOS Big Sur, use MacPro7,1 SMBIOS.

## What's working?
- Full Hardware Acceleration
- Audio (Speaker + Headphone)
- Ethernet
- External Devices
  - Webcam
  - Mic

## Bugs
- Memory Modules Misconfigured notification after login screen
  - This is a well known bug in macOS BigSur. You can ignore it. It's caused because of MacPro7,1 SMBIOS. If you're annoyed by this, follow this guide to fix the problem. 
  - https://dortania.github.io/OpenCore-Post-Install/universal/memory.html

## What's Not Working?
- Softwares using Intel Virtualization Technology
  - Android Emulators (use physical devices or Genymotion Android Emulator)
  - Docker Engine (there are workarounds but not recommended)
- Sleep (Fix: Disable sleep in System Preferences)

## Not Tested
- iServices (Facetime, iMessage...)
- Adobe Suite
- Wi-Fi & Bluetooth dongles

## Important Links
1. OpenCorePkg: https://github.com/acidanthera/OpenCorePkg
2. GenSMBIOS: https://github.com/corpnewt/GenSMBIOS
3. ProperTree: https://github.com/corpnewt/ProperTree
4. MountEFI: https://github.com/corpnewt/MountEFI
5. SSDTTime: https://github.com/corpnewt/SSDTTime
6. AMD Power Gadget(optional): https://github.com/trulyspinach/SMCAMDProcessor/releases

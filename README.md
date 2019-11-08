<p align="center">
 <img src="https://ibin.co/4wX5oSSZBLqt.png"/>
</p>

<p align="center">
 <img src="https://ibin.co/4wWyAVkKNTUv.png" width="383" height="46"/>
</p>

Tested with macOS Catalina 10.15, but should work with Mojave. iCloud, iMessage, FaceTime and Siri are all fully functional but flush a new SMBIOS if you decide to use this configuration. iMac 14,2 or iMacPro1,1 work best.

🌀 **Looking for [OpenCore?](https://github.com/willza3/macOS-strix-B450i/tree/OpenCore)**

## System Specifications

- **Motherboard:** Asus ROG Strix B450-I
  * Networking: Intel I211-AT
  * Audio Codec: ROG SupremeFX (S1220A)
  * Wireless: Asus WiFi GO!
  
- **CPU:** AMD Ryzen 3 2200G @ 3.5 GHz (Temporary)

- **GPU:** Sapphire Nitro+ Radeon RX 580 8GB

## BIOS Settings

For best results, load optimised defaults - BIOS Version 2801 (24/09/2019)

- SVM Mode -> Disabled (Can be enabled post-install)
- SATA Mode -> AHCI
- IOMMU -> Disabled
- XHCI Hand-off -> Enabled
- Boot\CSM -> Disabled
- Secure Boot -> Other OS

**Ryzen G CPU?** Disable CPB to help minimise against audio issues.

- Core Performance Boost -> Disabled

## Guides & Links

#### Guides
- [AIO Vanilla Hackintosh Guide](https://kb.hackintoshisfun.ml/clover/)
- [GPU Guide (Great for determining GPU settings)](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)

#### Links
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
- [Kext Repo](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)
- [Set busratio, CPU and Bus speeds](https://forum.amd-osx.com/viewtopic.php?t=3440)

## Known Issues

- Internal WiFi & Bluetooth are non-functional.

- FileVault can cause issues.

*8 November, 2019*

☘️
	

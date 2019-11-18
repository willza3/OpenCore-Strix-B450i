<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

⚠️ **OpenCore is in beta. This configuration could have issues.**

🍀 **Looking for [Clover?](https://github.com/willza3/macOS-strix-B450i/tree/Clover)**

Tested with macOS Catalina 10.15.1 but should work with Mojave. All iCloud services are fully functional, but flush a new SMBIOS if you decide to use this. Rather than compiling directly from source, this configuration uses the latest public release - which is currently 0.5.2.

## What is OpenCore?
OpenCore is an open-source bootloader, designed to be an alternative to Clover. OpenCore aims to resolve the constraints and issues imposed by Clover by providing a more versatile and modular system. While OpenCore is primarily designed for Hackintosh systems, it can be used in any scenario where an emulated EFI is needed. 

Please remember that OpenCore is still new and currently in beta. Unless you want to be on the bleeding edge of Hackintosh development or are planning on contributing to the project, you probably don't want to migrate if you have a stable system currently.

######(Taken from the OpenCore Vanilla Desktop Guide)

## System Specifications

- **Motherboard:** Asus ROG Strix B450-I
  * Networking: Intel I211-AT
  * Audio Codec: SupremeFX S1220A
  * Wireless: Realtek 8822BE
  
- **CPU:** AMD Ryzen 5 2600X
- **GPU:** Sapphire Nitro+ Radeon RX 580 8GB

## BIOS Settings

For best results, load optimised defaults - BIOS Version 2801 (24/09/2019)

- SVM Mode -> Disabled (Can be enabled post-install)
- SATA Mode -> AHCI
- IOMMU -> Disabled
- XHCI Hand-off -> Enabled
- Boot\CSM -> Disabled
- Secure Boot -> Other OS

**Ryzen G CPU?** Disabling CPB can help reduce audio issues.

- Core Performance Boost -> Disabled

## Guides & Links

#### Guides
- [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [Catalina GPU Guide](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)

#### Links

- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- [OpenCore Changelog](https://github.com/acidanthera/OpenCorePkg/blob/master/Changelog.md)
- [Kext Repo](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)
- [CPU Name](https://github.com/corpnewt/CPU-Name)


## Known Issues

- Internal WiFi & Bluetooth are not supported.

- FileVault is currently *un-tested.*

*18 November, 2019*

🌀
	
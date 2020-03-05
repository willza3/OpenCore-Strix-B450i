<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

⚠️ **OpenCore is still in beta. Please keep this in mind.**

🔔 **Join the Telegram [Channel](https://t.me/macOSstrixB450i) for the latest updates.**      

Tested with macOS Catalina 10.15.3, but expected to work with Mojave 10.14. This configuration uses OpenCore 0.5.6 - any later releases of OpenCore have not yet been tested so use at your own risk.

This configuration works out the box with iCloud services, but it's **highly reccomended to [flush a new SMBIOS.](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/amd-config.plist/amd-config#platforminfo)** Using the included SMBIOS could result in a blacklisted or permanently banned Apple ID.

## What is OpenCore?
OpenCore is an open-source unconventional first-in-class piece of software designed to intercept kernel loading to insert a highly advanced rootkit, designed to be an alternative to Clover. OpenCore aims to resolve the constraints and issues imposed by Clover by providing a more versatile and modular system. While OpenCore is primarily designed for Hackintosh systems, it can be used in any scenario where an emulated EFI is needed.

— From the OpenCore Vanilla Guide

## System Specifications

- **Motherboard:** Asus ROG Strix B450-I
  * Networking: Intel I211-AT
  * Audio Codec: SupremeFX S1220A (Layout 7)
  * Wireless: Realtek 8822BE
  
- **CPU:** AMD Ryzen 5 2600X
- **GPU:** Sapphire Nitro+ Radeon RX 580 8GB
    * Navi GPU? Add this boot flag: ```agdpmod=pikera```

## BIOS Settings

For best results, load optimised defaults - BIOS Version 2801 (24/09/2019)

- SVM Mode -> Disabled (Can be enabled post-install)
- SATA Mode -> AHCI
- IOMMU -> Disabled
- XHCI Hand-off -> Enabled
- Boot\CSM -> Disabled
- Secure Boot -> Other OS

**Ryzen G CPU?** Disable CPB to help reduce audio issues on Ryzen G CPUs.

- Core Performance Boost -> Disabled

## Guides & Links

#### Guides
- [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [Catalina GPU Guide](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)
- [Snazzy Labs' OpenCore Guide](https://youtu.be/l_QPLl81GrY)

#### Links

- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- [Kext Repo](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)
- [CPU Name](https://github.com/corpnewt/CPU-Name)
- [OpenCore Sanity Checker](https://opencore.slowgeek.com)


## Known Issues

- Internal WiFi & Bluetooth are not supported.

- Watching DRM-Protected Video (e.g Netflix) with Safari can cause a kernel panic.

- FileVault 2 should be properly supported as of early February 2020 builds, but **has not been properly tested.**

*4 March, 2020*

🌀
	

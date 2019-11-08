<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>

⚠️ **OpenCore is currently in early development. This configuration may have issues.**

🍀 **Looking for [Clover?](https://github.com/willza3/macOS-strix-B450i/tree/master)**

## What is OpenCore?
OpenCore is an alternative to the Clover bootloader. By design, OpenCore is versatile by being more modular and open as it aims to resolve the constraints and issues that Clover brings. Please remember we’re still in very early infancy so there will be issues. OpenCore should be considered in Alpha stage at this time. If you have a working, stable system you should not migrate unless you prefer "bleeding edge" development, want to contribute, and don't mind recovering your system should it fail to boot.

## System Specifications

- **Motherboard:** Asus ROG Strix B450-I
  * Networking: Intel I211-AT
  * Audio Codec: ROG SupremeFX (S1220A)
  * Wireless: Asus WiFi GO!
  
- **CPU:** AMD Ryzen 3 2200G @ 3.5 Ghz (Temporary)

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
- [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [Catalina GPU Buyers Guide (Great for determining settings)](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)

#### Links

- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- [OpenCore EFI Builder (Make sure to read the wiki)](https://github.com/rusty-bits/OC-tool)
- [Kext Repo](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)


## Known Issues

- Internal WiFi & Bluetooth are non-functional.

- FileVault *un-tested.*

*8 November, 2019*

🌀

<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

⚠️ **OpenCore is still in beta. Please keep this in mind.**

🛎 **Join the Telegram [Channel](https://t.me/macOSstrixB450i) for notifications about updates.**

Tested with macOS 10.15.4 SU1 with OpenCore 0.5.7 - any later versions of macOS and OpenCore have not yet been tested, so use them at your own risk. This configuration works with iCloud services, but it's **strongly recommended** to [flush a new SMBIOS.](https://dortania.github.io/OpenCore-Desktop-Guide/AMD/zen.html#platforminfo) Using the included one could result in a permanently banned Apple ID, which I can't be held responsible for.

## System Specification

* **Motherboard:** ASUS ROG Strix B450-I
	* Networking: Intel I211-AT
	* Audio: SupremeFX S1220A (ALC Layout 7)
	* Wireless: Realtek 8822BE (Stock)

* **CPU:** AMD Ryzen 5 2600X
* **GPU:** Sapphire Nitro+ Radeon RX 580 8GB

Dual-booted with Windows 10. OpenCore installed on macOS SSD and set as primary boot device for OpenCanopy.


## BIOS Settings
**For the best results, load *optimised defaults* and change the following options;**

* SVM Mode -> Disabled (Enable after install)
* SATA Mode -> AHCI
* IOMMU -> Disabled
* XHCI Handoff -> Enabled
* Boot/CSM -> Disabled
* Secure Boot -> Other OS

**Ryzen G CPUs using integrated audio:**

* Core Performance Boost -> Disabled

These settings were tested with BIOS v2801 (24/09/2019) - use the latest available version of your BIOS to mitigate any issues (in general).

## Known Issues

* **Internal WiFi & Bluetooth are not supported by macOS.**

Solution: The internal wireless card can be replaced with a compatible one, such as the Dell DW1820A. I haven't tried this myself, but there are reports of it working...

## Guides & Links

#### Guides

* [OpenCore Vanilla Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide)

* [Catalina GPU Guide](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)

* [Snazzy Labs' OpenCore Guide](https://youtu.be/l_QPLl81GrY)

#### Links

* [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)

* [OpenCore Sanity Checker](https://opencore.slowgeek.com)

#### Apps

* [AMD Power Gadget](https://github.com/trulyspinach/SMCAMDProcessor/releases)

* [External­Display­Brightness](https://github.com/fnesveda/ExternalDisplayBrightness/releases)

*19 April, 2020*

🌀
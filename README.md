<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

⚠️ **OpenCore is still in beta. Please keep this in mind.**

🛎 **Join the Telegram [Channel](https://t.me/macOSstrixB450i) for notifications about updates.**

Tested with macOS 10.15.5 SU with OpenCore 0.5.9 - any later versions of macOS and OpenCore have not yet been tested, so use them at your own risk. This configuration works with iCloud services, but it's **strongly recommended** to [flush a new SMBIOS.](https://dortania.github.io/OpenCore-Desktop-Guide/AMD/zen.html#platforminfo) Using the included one could result in a permanently banned Apple ID, which I can't be held responsible for.

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

#### Boot

* Fast Boot -> Disabled
* CSM -> Launch CSM -> Disabled
* Secure Boot -> OS Type -> Windows UEFI

#### Advanced
* USB Configuration -> XHCI Hand-off -> Enabled

**Ryzen G CPUs using integrated audio:**

* Core Performance Boost -> Disabled

These settings were tested with BIOS v3004 (27/12/2019) - use the latest available version of your BIOS to mitigate any issues (in general).

## Known Issues

**Internal WiFi & Bluetooth are not supported by macOS.**

* **Solution:** The internal wireless card can be replaced with a macOS compatible one (e.g Dell DW1820A). I haven't tried this myself, but there are reports of it working.

**Line-in microphones may not appear.**

* **Solution:** AppleALC has minimal support for line-in microphones on Ryzen/TR CPUs. Buying a USB adapter seems to be the best option at this time.

**Discord stuck in a crash loop.**

* **Solution:** [Fix here](https://discordapp.com/channels/249992304503291905/263798638373896203/717912500498333746) (Method 2 worked for me)

**Unable to wake from sleep.**

* **Solution:** No fix at the moment.

Sleep and Wake does not work if:

* USB 2.0 device plugged into the motherboard's USB 3.1 I/O ports.
* USB 2.0 device connected to a USB 3.0 hub and plugged into the motherboard's USB 3.1 I/O port, Sleep works if only the hub is plugged into a USB 2.0 I/O port.
* Auto sleep and hibernate won't work if an external mechanical hard drive is mounted in macOS.

**Please report any issues you find [here.](https://github.com/willza3/macOS-strix-B450i/issues)**

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

**Last Updated:** 4 June 2020

🌀

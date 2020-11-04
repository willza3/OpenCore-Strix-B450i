<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

⚠️ **OpenCore is still in beta. You may run into issues.**

🔔 **Telegram [Channel](https://t.me/macOSstrixB450i)**

Tested with macOS 10.15.7 ― later versions of macOS have not been tested. This EFI is not guaranteed to work flawlessly with your hardware, but it can be used as a starting point for getting your hackintosh up and running.

You will need to [flush a new SMBIOS](https://dortania.github.io/OpenCore-Desktop-Guide/AMD/zen.html#platforminfo) if you want to use iCloud services. The included SMBIOS is blacklisted and can result in a suspended Apple ID account.

If you're able to, please consider [donating to AMD OSX.](https://forum.amd-osx.com/index.php?dbtech-donate/drives/amd-os-x.1/donate). Without the team, this fun project wouldn't be possible!

## System Specs

* **Motherboard:** Asus Strix B450-I
	* LAN: Intel I211-AT
	* Audio: SupremeFX S1220A
	* Wireless: Realtek 8822BE
	* SSD: Sabrent Rocket 1TB NVMe

* **Processor:** AMD Ryzen 5 2600X
* **Graphics:** Sapphire Nitro+ AMD Radeon RX 580 8GB

## Reccomended BIOS Settings

Tested with BIOS v3004 - using the latest BIOS can reduce chances of issues.

**Boot**

* Fast Boot → Disabled
* CSM → Launch CSM → Disabled
* Secure Boot → OS Type → Windows UEFI

> Set OS Type to "Other" if you're having issues booting the macOS installer.

**Advanced**

* USB Configuration → XHCI Hand-off → Enabled

* Core Performance Boost → Disabled

> Ryzen G CPUs only - helps reduce audio crackling but won't fix it.

## Issues

**Internal WiFi & Bluetooth is not supported by macOS.**

* **Workaround:** The internal wireless card can be replaced with one that is compatible with macOS.

**Line-in microphones may not work.**

* **Workaround:** AppleALC does not support line-in microphones. Currently, the best option is to purchase a USB adapter.

**Unable to wake from sleep.**

* **Workaround:** [More details.](https://github.com/willza3/macOS-strix-B450i/issues/13#issuecomment-642053047) Thank you @conchodaus!

**Unable to open Discord.**

* **Fix:** [Link](https://discordapp.com/channels/249992304503291905/263798638373896203/717912500498333746)

**Last Updated:** 4 November 2020

🌀
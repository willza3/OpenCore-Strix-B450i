<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p>
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

Tested with macOS 11.0.1 - later versions have not been tested. This EFI isn't guaranteed to work flawlessly with your hardware... but it can be used as a starting point to aid getting your hackintosh up and running. Feel free to join my Telegram [channel](https://t.me/macOSstrixB450i).

You will need to [flush a new SMBIOS](https://dortania.github.io/OpenCore-Desktop-Guide/AMD/zen.html#platforminfo) if you want to use iCloud services. The included SMBIOS has been blacklisted and may result in a suspended iCloud account if you choose to use it.

If you're able to, please consider [donating to AMD OSX.](https://forum.amd-osx.com/index.php?dbtech-donate/drives/amd-os-x.1/donate) Without the team, this fun project wouldn't be possible!



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

**Last Updated:** 14 November 2020

🌀
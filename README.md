<p>
	<img src="https://ibin.co/5zbFfCb4uxve.png">
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

Tested with macOS 11.6.1 — later versions have not been tested. This EFI is not guaranteed to 100% work with your hardware... but it can be used as a starting point to get your machine up and running. Feel free to join the [Telegram](https://t.me/macOSstrixB450i) channel for discussion and updates.

You will need to [flush a new SMBIOS](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#platforminfo) if you wish to use iCloud services. The included SMBIOS is blank and will not work.

If you're able to, please consider [donating to AMD OS X.](https://forum.amd-osx.com/index.php?dbtech-donate/drives/amd-os-x.1/donate) Without the team, none of this would be possible!

## System Specs

* **Motherboard:** Asus Strix B450-I
	* LAN: Intel I211-AT
	* Audio: SupremeFX S1220A
	* Wireless: Realtek 8822BE
	* Bluetooth: Laird BT852 (USB)
	* SSD: Sabrent Rocket 1TB NVMe

* **Processor:** AMD Ryzen 5 2600X
* **Graphics:** Sapphire Nitro+ AMD Radeon RX 580 8GB

## BIOS Settings

Tested with BIOS 4301 (March 2021) - try upgrading to this version before troubleshooting any issues.

**Boot**

* Fast Boot → Disabled
* CSM → Launch CSM → Disabled
* Secure Boot → OS Type → Windows UEFI

> Set OS Type to "Other" if you're having issues booting the macOS installer.

**Advanced**

* USB Configuration → XHCI Hand-off → Enabled

* Core Performance Boost → Disabled

> For Ryzen G CPUs only - helps reduce audio crackling but **won't** fix it.

## Known Issues

**Internal WiFi & Bluetooth is not working.**

* **Fix:** The internal wireless card can be replaced with one that is compatible with macOS.

**Discord stuck in a crash loop.**

* **Fix:** [Here](https://www.reddit.com/r/hackintosh/comments/g6bwuu/discord_keeps_crashing_every_time_i_join_a_voice/fv43nwi?utm_source=share&utm_medium=web2x&context=3)

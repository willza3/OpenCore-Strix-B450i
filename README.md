<p align="center">
	<img src="https://ibin.co/52IbeCHLerMK.png"/>
</p>

<p align="center">
	<img src="https://ibin.co/4wROyHBs3PAE.png" width="383" height="46"/>
</p>

⚠️ **OpenCore is still in beta. You may run into issues.**

🔔 **Join the Telegram [Channel](https://t.me/macOSstrixB450i) for updates.**

Tested with macOS 10.15.6 b2 - any later versions of Catalina have not been tested so use them at your own risk! Check the branches for Big Sur support.

If you would like to use iCloud services, you will need to [flush a new SMBIOS](https://dortania.github.io/OpenCore-Desktop-Guide/AMD/zen.html#platforminfo). Using the included one is unsafe and can result in a permenantly blacklisted Apple ID - *you have been warned!*

If you can, please consider [donating to AMD OSX.](https://forum.amd-osx.com/index.php?dbtech-donate/drives/amd-os-x.1/donate) Without the team, none of this would be possible.

## System Specs

* **Motherboard:** Asus Strix B450-i
	* LAN: Intel I211-AT
	* Audio: SupremeFX S1220A
	* Wireless: Realtek 8822BE

* **Processor:** AMD Ryzen 5 2600X
* **Graphics:** Sapphire Nitro+ AMD Radeon RX 580 8GB

## Reccomended BIOS Settings

**Boot**

* Fast Boot → Disabled
* CSM → Launch CSM → Disabled
* Secure Boot → OS Type → Windows UEFI

> Set OS Type to "Other" if you're having issues booting the macOS installer.

**Advanced**

* USB Configuration → XHCI Hand-off → Enabled

**Using a Ryzen G CPU?**

* Core Performance Boost → Disabled

These settings were tested with BIOS v3004 - use the latest available BIOS to mitigate any issues.

## Issues

**Internal WiFi & Bluetooth is not supported by macOS.**

* **Workaround:** The internal wireless card can be replaced with one that is compatible with macOS.

**Line-in microphones may not work.**

* **Workaround:** AppleALC does not support line-in microphones. Currently, the best option is to purchase a USB adapter.

**Unable to wake from sleep.**

* **Workaround:** [More details.](https://github.com/willza3/macOS-strix-B450i/issues/13#issuecomment-642053047) Thank you @conchodaus!

**Discord gets stuck in a crash loop.**

* **Fix:** [Link](https://discordapp.com/channels/249992304503291905/263798638373896203/717912500498333746)

**Last Updated:** 26 June 2020

🌀
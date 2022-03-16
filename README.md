<p>
	<img src="banner.png">
</p>

Tested with macOS 12.3 – later versions have not been tested. This EFI is my personal configuration and is not 100% guaranteed to work with your hardware... but is intended to be used as a reference point to get your hackintosh up and running. Feel free to join the [Telegram](https://t.me/macOSstrixB450i) chat for discussion. Please note that you'll need to [flush a new SMBIOS](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#platforminfo) if you wish to use iCloud services. The included SMBIOS is intentionally blank.

If you're able to, please consider [donating directly to AMD OS X!](https://forum.amd-osx.com/index.php?dbtech-donate/drives/amd-os-x.1/donate) Without the talented team and forums, this fun would not be possible. 

## BIOS Settings

Tested with BIOS 4602 (September 2021) - try upgrading to this version before troubleshooting any issues.

**Boot**

* Fast Boot → Disabled
* CSM → Launch CSM → Disabled
* Secure Boot → OS Type → Windows UEFI

> Set OS Type to "Other" if you're having issues booting the macOS installer.

**Advanced**

* USB Configuration → XHCI Hand-off → Enabled

* Core Performance Boost → Disabled

> For Ryzen G CPUs only - helps reduce audio crackling but **won't** fix it.

## Reference Specifications

* **Motherboard:** Asus Strix B450-I
	* LAN: Intel I211-AT
	* Audio: SupremeFX S1220A (ALC1150 Codec)
	* Wireless: Realtek 8822BE
	* Bluetooth: Laird BT852 (USB)
	* SSD: Sabrent Rocket 1TB NVMe

* **Processor:** AMD Ryzen 5 2600X
* **Graphics:** Sapphire Nitro+ AMD Radeon RX 580 8GB

## Common Questions

**My audio isn't working!**

* Certain revisions of this motherboard, either for the Chinese market or those produced around mid-late 2021 have a different device path for the multimedia controller. Try changing the path in your config.plist from ```PciRoot(0x0)/Pci(0x8,0x1)/Pci(0x0,0x3)``` to ```PciRoot(0x0)/Pci(0x8,0x1)/Pci(0x0,0x4)```

**My internal WiFi & Bluetooth isn't working!**

* The internal wireless card is not natively compatible, but can be replaced with one that is compatible with macOS.

**My Discord stuck in a crash loop!**

* [Solution here](https://discord.com/channels/249992304503291905/283346899799638016/953634716479799297) (Opens AMD OS X Discord) I highly reccomend becoming part of this server if you are not already!

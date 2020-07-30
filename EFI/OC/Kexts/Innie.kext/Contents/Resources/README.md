Innie
=====

A [Lilu](https://github.com/acidanthera/Lilu) plugin for making PCIe drives appear as internal. The plugin is compatible with Lilu 1.2.0 or later.
  
#### Configuration

- `-inniedbg` enables debug printing (available in DEBUG binaries).
- `-innieoff` disables the plugin.
- `-inniebeta` enables the plugin on macOS versions newer than Catalina.

#### Alternative

An alternative to Innie is to add the `built-in` device property for each drive. This can be accomplished with [OpenCore](https://github.com/acidanthera/OpenCorePkg).

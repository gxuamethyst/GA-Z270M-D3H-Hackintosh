# OpenCore config for Gigabyte Z270M-D3H hackintosh

Base generated by [OC-Gen-X(version 3.3.2)](https://github.com/Pavo-IM/OC-Gen-X).

## Hardware

* Motherboard: Gigabyte GA-Z270M-D3H
* CPU: Intel Core i5-7500(Kaby Lake)
* Graphics Card: Sapphire RX560XT 4GB(with Intel HD Graphics 630)
* RAM: Crucial Ballistix Sport LT (8GB) x 2
* SSD: Samsung 850 EVO M.2 250GB
* Monitor: Acer EK241QK (3840 x 2160)

## OS

* Apple macOS Monterey 14.0 (23A344)

> verified on macOS 10.15.x, 11.x, 12.x, 13.x, 14.x
>
> if can not download 14.x from app store, please use gibMacOS instead.

## BIOS

* version **F8d**, you can download the latest version from [Gigabyte](https://www.gigabyte.cn/Motherboard/GA-Z270M-D3H-rev-10/support#support-dl-bios).
* BIOS settings

> 1. <u>Save & Exit</u> : *Load Optimized Defaults*
> 2. <u>M.I.T.</u> : Advanced Memory Settings → Extreme Memory Profile(X.M.P.) : *Profile1*
> 3. <u>BIOS</u> → Fast Boot : *Disabled*
> 4. <u>BIOS</u> → Windows 8/10 Features : *Other OS*
> 5. <u>BIOS</u> → LAN PXE Boot Option ROM : *Disabled*
> 6. <u>BIOS</u> → Storage Boot Option Control : *UEFI*
> 7. <u>Peripherals</u> → Initial Display Output : *IGFX*(for Intel GPU) or *PCIe 1 Slot*(for AMD GPU)
> 8. <u>Peripherals</u> → Super IO Configuration → Serial Port : *Disabled*
> 9. <u>Peripherals</u> → Super IO Configuration → Parallel Port : *Disabled*
> 10. <u>Peripherals</u> → Network Stack Configuration → Network Stack : *Disabled*
> 11. <u>Peripherals</u> → USB Configuration → Legacy USB Support : *Disabled*
> 12. <u>Peripherals</u> → USB Configuration → XHCI Hand-off : *Enabled*
> 13. <u>Power</u> → Platform Power Management : *Disabled*
> 14. <u>Chipset</u> → Vt-d : *Disabled*
> 15. <u>Chipset</u> → Wake on LAN Enable : *Disabled*
> 16. <u>Chipset</u> → Internal Graphics : *Enabled*(for hardware acceleration support)
> 17. Press *F10* to Save and Exit the BIOS

## OpenCore

* version **0.9.5**, you can download the latest version from [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg/releases).

## Drivers

* OpenRuntime.efi(Builtin by OpenCore)
* [HfsPlus.efi](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)

## Kexts

* [VirtualSMC](https://github.com/acidanthera/virtualsmc/releases)
* [Lilu](https://github.com/acidanthera/Lilu/releases)
* [IntelMausi](https://github.com/acidanthera/IntelMausi/releases)
* [AppleALC](https://github.com/acidanthera/AppleALC/releases)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)
* ~~USBPorts.kext(customized with [USBInjectAll.kext](https://bitbucket.org/RehabMan/os-x-usb-inject-all) via [Hackintool](https://github.com/headkaze/Hackintool), please check [https://blog.csdn.net/LeoForBest/article/details/103247824](https://blog.csdn.net/LeoForBest/article/details/103247824))~~
* USBToolBox.kext
  * [https://github.com/USBToolBox/tool](https://github.com/USBToolBox/tool)
  * [https://github.com/USBToolBox/kext](https://github.com/USBToolBox/kext)
* [AGPMInjector.kext](https://github.com/Pavo-IM/AGPMInjector)(Builtin by OC-Gen-X)

## Tools

* [OC-Gen-X](https://github.com/Pavo-IM/OC-Gen-X/releases): generate OpenCore config
* [Clover Configurator](https://mackie100projects.altervista.org/download/clover-configurator-global-edition/): mount EFI partition
* [OpenCore Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/): edit config.plist
* [Hackintool](https://github.com/headkaze/Hackintool/releases): check hackintosh info
* [Intel Power Gadget](https://www.intel.com/content/www/us/en/developer/articles/tool/power-gadget.html): check CPU status
* [VideoProc Converter](https://www.videoproc.com/): check hardware acceleration status
* [USBToolBox](https://github.com/USBToolBox/tool/releases): for USB customized

## Working

* CPU(Intel Turbo Boost)
* GPU(hardware acceleration)
* Audio
* Ethernet
* USB 2.0 & USB 3.0
* Sleep & Wake Up
* Facetime & iMessage

> without WiFi or Bluetooth.

## Others

> Note: You need a USB 2.0 Flash Drive for this motherboard.
> A USB 3.0 Flash Drive will cause a kernel panic when trying to load the installer because the rear ports on this motherboard are all USB 3.1 ports which cannot run 3.0 devices during the installation process on the Z270 Chipset.

## References

* [https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf)
* [https://oc.skk.moe/](https://oc.skk.moe/)
* [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
* [https://heipg.cn/tutorial/one-key-opencore-efi.html](https://heipg.cn/tutorial/one-key-opencore-efi.html)
* [https://opencore.slowgeek.com/](https://opencore.slowgeek.com/)
* [https://github.com/corpnewt/gibMacOS](https://github.com/corpnewt/gibMacOS)

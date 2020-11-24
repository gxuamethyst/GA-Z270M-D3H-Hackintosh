# OpenCore config for Z270M-D3H hackintosh

Base generate by [OC-Gen-X](https://github.com/Pavo-IM/OC-Gen-X).

## Hardware

* Motherboard: Gigabyte GA-Z270M-D3H
* CPU: Intel Core i5-7500
* Graphics Card: Sapphire RX560XT 4GB
> recognized with 'Radeon RX 470 4 GB' in Hackintosh
* RAM: Crucial Ballistix Sport LT (8GB) x 2
* SSD: Samsung 850 EVO M.2 250GB
* Monitor: Acer EK241QK (3840 x 2160)

## OS

* Apple macOS Big Sur 11.0.1(20B50)

## BIOS

* version F8d, you can download the latest version from [Gigabyte](https://www.gigabyte.com/Motherboard/GA-Z270M-D3H-rev-10#support-dl-bios).
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
> 16. Press *F10* to Save and Exit the BIOS

## OpenCore

* version 0.6.3, you can download the latest version from [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg/releases).

## Kexts

* [VirtualSMC](https://github.com/acidanthera/virtualsmc/releases)
* [Lilu](https://github.com/acidanthera/Lilu/releases)
* [IntelMausi](https://github.com/acidanthera/IntelMausi/releases)
* [AppleALC](https://github.com/acidanthera/AppleALC/releases)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)
* USBPorts.kext(custom with [USBInjectAll.kext](https://bitbucket.org/RehabMan/os-x-usb-inject-all), check [https://blog.csdn.net/LeoForBest/article/details/103247824](https://blog.csdn.net/LeoForBest/article/details/103247824))

## Others

> Note: You need a USB 2.0 Flash Drive for this motherboard. A USB 3.0 Flash Drive will cause a kernel panic when trying to load the installer because the rear ports on this motherboard are all USB 3.1 ports which cannot run 3.0 devices during the installation process on the Z270 Chipset.

> migrate from Clover?
> 
> check:
> 
> https://github.com/dortania/OpenCore-Install-Guide/tree/master/clover-conversion#cleaning-the-clover-junk-in-macos
> https://blog.skk.moe/post/from-clover-to-opencore/#%E6%B8%85%E7%90%86-Clover-%E6%AE%8B%E4%BD%99

## References

* [https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf)
* [https://oc.skk.moe/](https://oc.skk.moe/)
* [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
* [https://heipg.cn/tutorial/one-key-opencore-efi.html](https://heipg.cn/tutorial/one-key-opencore-efi.html)
* [https://heipg.cn/tutorial/example-of-from-clover-to-opencore.html](https://heipg.cn/tutorial/example-of-from-clover-to-opencore.html)
* [https://blog.skk.moe/post/from-clover-to-opencore/](https://blog.skk.moe/post/from-clover-to-opencore/)
* [https://blog.daliansky.net/OpenCore-BootLoader.html](https://blog.daliansky.net/OpenCore-BootLoader.html)
* [https://opencore.slowgeek.com/](https://opencore.slowgeek.com/)
* [https://github.com/Pavo-IM/OC-Gen-X](https://github.com/Pavo-IM/OC-Gen-X)

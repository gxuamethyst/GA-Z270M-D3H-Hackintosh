# Clover config for Z270M-D3H hackintosh

Base on [EFI-Pack-GA-Z270M-D3H.zip](http://hackintosher.com/wp-content/uploads/2017/06/EFI-Pack-GA-Z270M-D3H.zip), see [GIGABYTE GA-Z270M-D3H HACKINTOSH BUILD GUIDE](https://hackintosher.com/builds/ga-z270m-d3h/).

## Hardware

* Motherboard: Gigabyte GA-Z270M-D3H
* CPU: Intel Core i5-7500
* Graphics Card: Gigabyte GeForce GTX 1060 G1 Gaming 3GB
* RAM: Crucial Ballistix Sport LT (8GB) x 2
* SSD: Samsung 850 EVO M.2 250GB
* Monitor: Dell UltraSharp U2518D (2560 x 1440)

## OS

* Apple macOS 10.13.6 High Sierra

## BIOS

* version F8b, you can download the latest version from [Gigabyte](https://www.gigabyte.com/Motherboard/GA-Z270M-D3H-rev-10#support-dl-bios).
* BIOS settings

> 1. <u>Save & Exit</u> : *Load Optimized Defaults*
> 2. <u>M.I.T.</u> : Advanced Memory Settings → Extreme Memory Profile(X.M.P.) : *Profile1*
> 3. <u>BIOS</u> → Fast Boot : *Disabled*
> 4. <u>BIOS</u> → Windows 8/10 Features : *Other OS*
> 5. <u>BIOS</u> → LAN PXE Boot Option ROM : *Disabled*
> 6. <u>BIOS</u> → Storage Boot Option Control : *UEFI*
> 7. <u>Peripherals</u> → Initial Display Output : *IGFX*(for intel gpu) or *PCIe 1 Slot*(for nvidia gpu)
> 8. <u>Peripherals</u> → Super IO Configuration → Serial Port : *Disabled*
> 9. <u>Peripherals</u> → Network Stack Configuration → Network Stack : *Disabled*
> 10. <u>Peripherals</u> → USB Configuration → XHCI Hand-off : *Enabled*
> 11. <u>Chipset</u> → Vt-d : *Disabled*
> 12. <u>Chipset</u> → Wake on LAN Enable : *Disabled*
> 13. Press *F10* to Save and Exit the BIOS

## Clover

* version r4674, you can download the latest version from [Clover EFI bootloader](https://sourceforge.net/projects/cloverefiboot/files/Installer/).

## Kexts

* [AppleALC](https://github.com/acidanthera/AppleALC/releases)
* [FakeSMC](https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/)
* [IntelMausiEthernet](https://bitbucket.org/RehabMan/os-x-intel-network/downloads/)
* [Lilu](https://github.com/acidanthera/Lilu/releases)
* [USBInjectAll](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)
* [XHCI-200-series-injector](https://github.com/RehabMan/OS-X-USB-Inject-All/archive/master.zip)

## Others

* [NVIDIA Drivers](https://www.tonymacx86.com/nvidia-drivers/)
* [one-key-hidpi](https://github.com/boboidream/one-key-hidpi)

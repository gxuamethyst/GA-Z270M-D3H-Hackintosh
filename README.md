# Clover config for Z270M-D3H hackintosh

Base on [EFI-Pack-GA-Z270M-D3H.zip](http://hackintosher.com/wp-content/uploads/2017/06/EFI-Pack-GA-Z270M-D3H.zip), see [GIGABYTE GA-Z270M-D3H HACKINTOSH BUILD GUIDE](https://hackintosher.com/builds/ga-z270m-d3h/).

## Hardware

* Motherboard: Gigabyte GA-Z270M-D3H
* CPU: Intel Core i5-7500
* Graphics Card: Sapphire RX560XT 4GB
* RAM: Crucial Ballistix Sport LT (8GB) x 2
* SSD: Samsung 850 EVO M.2 250GB
* Monitor: Acer EK241QK (3840 x 2160)

## OS

* Apple macOS 10.15.6 Catalina(19G73)

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

## Clover

* version r5119, you can download the latest version from [Clover EFI bootloader](https://github.com/CloverHackyColor/CloverBootloader/releases).

## Kexts

* [VirtualSMC](https://github.com/acidanthera/virtualsmc/releases)
* [Lilu](https://github.com/acidanthera/Lilu/releases)
* [IntelMausi](https://github.com/acidanthera/IntelMausi/releases)
* [AppleALC](https://github.com/acidanthera/AppleALC/releases)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)

## References

* [GIGABYTE GA-Z270M-D3H HACKINTOSH BUILD GUIDE](https://hackintosher.com/builds/ga-z270m-d3h/)
* [Hackintosh Vanilla Desktop Guide](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/)

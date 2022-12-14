MSI-MAG-B6660m Mortar (no-Wi-Fi)-DDR4-i5 12600k-RX6600XT-EFI

## My specs

| Spec | Model |
| --- | --- |
| CPU | [Intel i5 12600K] |
| Mainboard | [MSI MAG B660M MORTAR DDR4 wihtout Wi-Fi] |
| VGA | [Gigabyte Radeon RX 6600XT Eagle] |
| RAM | Corsair Vengeance RGB RS 32GB 3200MHz DDR4 (4x8GB) CMG16GX4M2E3200C16 |
| Wireless card | BCM94360CD |
| SSD | Samsung PM961 |
| OC | 0.8.7 |
| macOS | macOS Ventura 13.1 |
| SMbios | MacPro 7,1 |

You need to re-select SMBios in Opencore Configurations (MacPro 7,1) to generate your Serial and system UUID...

![Screenshot 2022-12-14 at 3.26.47 PM.png](https://github.com/haianhlc99/-MSI-MAG-B6660m-Mortar-no-Wi-Fi--DDR4-i5-12600k-RX6600XT-EFI/blob/2950a6733ad3fa7fec5b2f2978845ed0eac9615c/Screenshot%202022-12-14%20at%203.26.47%20PM.png)

![Screenshot 2022-12-14 at 3.26.56 PM.png](https://github.com/haianhlc99/-MSI-MAG-B6660m-Mortar-no-Wi-Fi--DDR4-i5-12600k-RX6600XT-EFI/blob/76c58bbba33c4062f739e4a541d2ae8c1e727636/Screenshot%202022-12-14%20at%203.26.56%20PM.png)

## BIOS configurations

This guide is applicable to B660M mortar motherboard, the motherboard BIOS needs the following settings, please update the bios to the latest version 7D42v17 and above

- Save & Exit → Restore Defaults : Yes
- Settings - Boot - Turn off Msi Fast Boot, Fastboot
- Settings - Security - Secureboot - Disabled
- Settings - Security - Trusted Computing - Security Device Support - Disabled
- Settings - Security - Trusted Computing - TPM Device Selection - PTT
- Setting - Advanced - Intergrated Graphics Configuration - Graphic adapter - PEG, IGD Multi Monitor - Disabled (This makes sleep does not work)
- Settings - Advanced - Integrated Peripherals - Network Stack - Disabled
- Settings - Advanced - Integrated Peripherals  - Intel Serial IO - Disabled
- Settings - Advanced - PCIe/PCI Sub-System Settings - Re-Size BAR Support- Enabled
- Settings - Advanced - USB Configuration - XHCI Hand-off - Enabled
- Settings - Advanced - USB Configuration - Legacy USB Support - Auto
- OC - Extreme Memory Profile (Xmp) - Enabled
- OC - Cpu Features - Turn off VT-d Tech, CFG Lock, Turn on Intel Virtualization Tech
- BETA - D.T.M - Enabled
- BETA - SR-IOV Support - Enabled

Wake from Keyboard Optional:
- Setting - Advanced - Power Management Setup - ErP Ready - Enable
- Setting - Advanced - Power Management Setup - USB Standby Power at S4/S5 - Enable
- Setting - Advanced - Resume By USB Device - Enable

Work:
- QE/CI of Gigabyte RX 6900 XT (XTXH)
- Restart, Sleep and Shutdown
- CPU Power Management
- Ethernet
- Rear and front Jack Audio
- HDMI/DP
- HDMI/DP Audio
- All USB Ports
- RX 6600 XT on macOS: Zero RPM with SoftPowerPlayTable 
- Etc

## Credits

- https://github.com/yzchan/MSI-MAG-B660M-MORTAR-DDR4-12600K-EFI
- https://www.tonymacx86.com/threads/rx-6600-xt-on-macos-zero-rpm-with-softpowerplaytable.319638/?fbclid=IwAR2ixTPROPm5iHmusTycbSEII7p9rQ5SwhSd6rbc2owSvibzfPEpla5hYeo

## Links

- [OC Auxiliary Tools](https://github.com/ic005k/QtOpenCoreConfig)
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [Hackintool](https://github.com/headkaze/Hackintool)
- [OpenCore](https://dortania.github.io/OpenCore-Install-Guide/prerequisites.html)
- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- https://blog.daliansky.net/
- https://apple.sqlsec.com/
- https://space.bilibili.com/16323318/channel/collectiondetail?sid=296068
- https://bbs.pcbeta.com/forum.php?gid=86
- https://www.tonymacx86.com/
- https://github.com/daliansky/OC-little

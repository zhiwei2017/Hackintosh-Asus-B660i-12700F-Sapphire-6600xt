# Introduction

This EFI uses OpenCore 0.8.6 and is used for install Hackintosh Monterey 12.6.1.
Please make sure the system matches to the one you want, before using it.

One of the most important reason I choose MacOS Monterey 12.6.1 is the stability.
Currently Hackintosh with MacOS Ventura 13.1 is still unstable.

# Version

macOS Monterey 12.6.1
OpenCore: 0.8.6 (RELEASE)

# Hardware specs


| MotherBoard        | Asus B660i                                      |
| -------------------- | ------------------------------------------------- |
| CPU                | Intel 12700F                                    |
| GPU                | Sapphire Nitro+ Radeon RX 6600 XT               |
| RAM                | Corsair Vengeance schwarz DIMM Kit 64GB         |
| SSD                | Western Digital WD_BLACK SN850 NVMe SSD 1TB * 2 |
| Wireless WIFI Card | BCM94360Z3                                      |
| PSU                | Corsair SF750                                   |

# What works

+ macOS Monterey
+ Shutdown
+ Reboot
+ Sleep
+ HDMI/DP
+ Ethernet
+ Wifi/BT
+ USB Ports
+ Audio
+ AirDrop/Handoff/Unlock with Apple Watch... (All Continuity features except Sidecar)
+ DRM

# What doesn't work

# To use this EFI

1. Check `https://dortania.github.io/OpenCore-Install-Guide/`_ for making MacOS installation USB drive.
2. In the section of **Config**, use the provided EFI to replace the one from USB drive.
3. Replace the default wireless card intel AX201 with BCM94360Z3.
4. Connect all the hardware components.
5. Check the section of **Installation** to install MacOS in your new PC.

# BIOS Setup

+ Advanced > CPU Configuration > Intel (VMX) Virtualization Technology > Enabled (defalut)
+ Advanced > CPU Configuration > Active Performance Cores > All (i5 12400f have no E-Cores, unknown)
+ Advanced > CPU Configuration > Hyper-Threading > Enabled (defalut)
+ Advanced > System Agent (SA) Configuration > VT-d > Enabled (defalut)
+ Advanced > System Agent (SA) Configuration > Control Iommu Pre-boot Behavior > Disable IOMMU (default? not sure)
+ Advanced > PCI Subsystem Settings > Above 4G Decording > Enabled (defalut)
+ Advanced > PCI Subsystem Settings > Re-Size BAR Support > Enabled (defalut)
+ Advanced > USB Configuration > Legacy USB Support > Enabled
+ Advanced > USB Configuration > XHCI Hand-off > Enabled
+ Advanced > Network Stack Configuration > Network Stack > Disabled
+ Advanced > USB Configuration > Legacy USB Support > Enabled
+ Boot > CSM (Compatibility Support Module) > Launch CSM > Disabled
+ Boot > Secure Boot > OS Type > Other OS
+ Boot > Secure Boot Mode > Custom
+ Boot > Boot Configuration > Fast Boot > Disabled

# Screenshots

![system_info](images/system_info.png)
![geekbench_score](images/geekbench_score.png)
![bluetooth](images/bluetooth.png)

# Thanks/Credits

- [Opencore Team](https://dortania.github.io/getting-started/)

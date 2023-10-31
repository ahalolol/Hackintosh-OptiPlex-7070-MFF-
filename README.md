# Hackintosh-OptiPlex-7070-MFF
![](https://github.com/ahalolol/Hackintosh-OptiPlex-7070-MFF-/blob/main/about.png)

**Opencore Bootloader 0.9.5. Tested on Sonoma 14.1**


## Introdution
This is the Hackintosh EFI Folder for Dell OptiPlex 7070 Micro Form Factor. 
This is built based on https://github.com/webleon/Hackintosh-OptiPlex-7070-MFF with new Config fitting Opencore 0.9.5 and recommendations found on the Opencore Tutorial.
You will have to [**generate a new SMIBIOS**](https://github.com/corpnewt/GenSMBIOS) before login to your iCloud account.


## Hardware Specs
* **Desktop Computer**: Dell OptiPlex 7070 Micro Form Factor 65W
* **CPU**: Intel® Core™ i7-9700
* **iGPU**: Intel® UHD Graphics 630
* **RAM**: 32GB DDR4 2666 Daul Channel
* **HDD**: TOSHIBA KBG40ZNT512G 
* **LAN**: Intel I219LM7
* **Wi-Fi & Bluetooth**: Intel AC9560


## Hardware Status
* CPU Turbo Boost & Thermal Throttling
* DP & HDMI
  * Single video out OK
  * Untested audio but device listed
  * Untested dual video
* iGPU acceleration
* Front panel Headset Line-out
  * Untested combo jack mic in
* All USB Ports
* Wireless & Bluetooth
  * Untested LAN but device recognized
* Sleep & Wakeup
* OTA via builtin software updater




## BIOS Settings
BIOS version is 1.22
* General → Advanced Boot Options: ***uncheck***
* System Configuration → SATA Operation: ***AHCI***
* Secure Boot → Secure Boot Enable: ***Disabled***
* Intel® Software Guard Extensions™ → Intel® SGX™ Enable: ***Disabled***
* Virtualization Support → VT for Direct I/O: ***uncheck***


## BIOS Settings via GRUB
* Set Pre-Allocated DVMT to 64M: 
***setup_var 0x8DC 0x02***
* Disable CFG lock: 
***setup_var 0x5BE 0x00***

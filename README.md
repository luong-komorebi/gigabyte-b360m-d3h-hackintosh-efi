#Hackintosh Mojave Installation Guide for Gigabyte B360M D3H Hackintosh & Clover EFI Folder

⚠️  **Please Read the whole readme file for better understanding. Also I will share some tips and tricks.**

### **What's Working?**

- Sleep/Wake
- Ethernet
- Audio ALC892 (native AppleALC audio)
- iGPU Quick Sync + RX 560 GPU
- All USB ports (USB 2 + USB 3)

    ![](/Screenshots/about.png)


- CPU: Intel i3 8100 
- Motherboard: Gigabyte B360M-D3H 
- Memory: Crucial DDR4 8GB x 2 
- GPU: Gigabyte Radeon RX 560 4GB OC
- Power supply: Gigabyte GP-PB500
- Case: Cooler Master Masterbox Q300L
- SSD: Crucial MX500 8GB x 2

### Install Guide
Reddit Vanilla install: https://www.reddit.com/r/hackintosh/comments/9i2ntq/vanilla_guide_make_macosx_installer_from_windows/ + some custom tweaked EFI

### Additional bios Settings: 
	•	Load optimised default 
	•	Disable CSM 
	•	Disable Fast 
	•	Enable Internal Graphics & VT-D 
	•	Disable only serial port (first option) 

After Installing MacOS on your system copy my clover folder to your EFI Partition and Open the config.plist make sure you set the following:
- SerialNumber
- BoardSerialNumber
- SmUUID

**Also Depending on your CPU Choose the Right SMBIOS.**
After Installing MacOS on your system copy my clover folder to your EFI Partition and Open the config.plist make sure you do the following:

- Set SMBIOS to **iMAC 18'2** or **iMAC 19'2** for i3-8100 (*Depending on your CPU Choose the Right SMBIOS)*
- Get a Patched DSDT.aml for your hackintosh from [Olarila Forum](https://olarila.com/forum/viewtopic.php?t=6401) (Must Needed for a stable and working hackintosh)
- Update the Kext to the latest version
- Generate  in Clover Configurator: **SerialNumberBoard, SerialNumber, SmUUID**

**💡 The Setup is 100% Stable! I have never faced any kernel panic or reboot.**

### Post Installation Tips

## Links:

[How to Stay within 15 ports limit using UsbInjectall and Clover boot argument](https://olarila.com/forum/viewtopic.php?f=79&t=7370&fbclid=IwAR0aba59fTABiOx2hLesroLLHOTl8rAQQwQ-d0bpPm4LZ3UNovBrGdjyEb8)

[[Guide] Easy Audio Solution with AppleAlc](https://olarila.com/forum/viewtopic.php?f=28&t=9788)

[HACKINTOSH IMESSAGE + ICLOUD + FACETIME REPAIR GUIDE](https://hackintosher.com/guides/quick-fixes-facetime-icloud-imessage-hackintosh-not-working/)

[Hide Volumes / Extra Boot Entries With Clover Config](https://olarila.com/forum/viewtopic.php?f=28&t=7451#p66199)


Intel Quick Sync Works
### Screenshots

![Quick Sync](/Screenshots/quicsync.png)
![Audio](/Screenshots/audio.png)
![Ethernet](/Screenshots/ethernet.png)
![Graphics](/Screenshots/graphics.png)
![USB 3](/Screenshots/usb.png)

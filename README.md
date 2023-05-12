# Dell Vostro 3590 OpenCore EFI 
<p align="center">
  <img src="https://i.imgur.com/t2i2ltB.png"/>
</p>

## Specifications :  

Device | Status | Details |
------------ | ------------- | ------------- | 
CPU | Working | **Intel(R) Core(TM) i5-10210U CPU @ 1.60GHz** |
Graphic | Working | Intel UHD620 |
SSD | Working | KIOXIA BG4 KBG40ZNS256G |
WiFi | Not Working | Qualcomm QCA9377 |
Card Reader | Not Tested | I don't know model |
Camera | Working | I don't know model |
Audio | Working | Realtek ALC3204 |
Touchpad | Working | I don't know model |
HDMI | Working | Thanks to [semba90](https://www.reddit.com/r/hackintosh/comments/zf5m2g/comment/iza65jq/?utm_source=share&utm_medium=web2x&context=3) |
USB Ports | Working | USB is mapped |
OS | Working | MacOS 12 Monterey |
Sleep | Not Working| Crashes macOS |
DRM | Can Work | Works with unfairgva=7 but system is laggy |

## Setting Up 

1. Place the EFI folder to the EFI partition

2. Generate your own SMBIOS :

- Do the following one line at a time in Terminal:
```
    git clone https://github.com/corpnewt/GenSMBIOS
    cd GenSMBIOS
    chmod +x GenSMBIOS.command
```
    
- Then run with either `python ./GenSMBIOS.command` on *nix system or by double-clicking *GenSMBIOS.command* on macOS.
On Windows `./GenSMBIOS.bat`.

- Choose *Install/Update MacSerial*.

- Then choose *Select the config.plist file* and select it from the EFI folder. 

- Now choose *Generate SMBIOS* and generate the SMBIOS by entering MacBookPro16,2

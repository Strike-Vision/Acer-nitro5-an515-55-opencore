## Acer nitro 5 an515-55 core i5 10300H gtx 1650 Ti opencore EFI

Sharing my OpenCore EFI for others to create their own hackintosh.
## Installation

[Follow these steps to creat the macos installer](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#downloading-macos) (skip setting up the EFI) Copy my EFI folder to your EFI partition and change the PlatformInfo in config.plist, Follow this [guide](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo) to do so (you will need [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and [ProperTree](https://github.com/corpnewt/ProperTree) when using GenSMBIOS the mac type should be: MacBookPro16,1)

## Optional (after installation)

remove verbose screen output (text on boot) edit the config.plist, go to NVRAM -> Add -> 7C436110-AB2A-4BBB-A880-FE41995C9F82 and remove -v from boot-args.

## Whats Working

- WiFi
- iGPU
- Battery Levels
- All USB Ports
- Trackpad - I2C
- Internal Keyboard
- Boot Chime
- Speakers
- Microphone
- iServices (You will need to follow this [guide](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios) to get it working)
- Brightness Control
- WebCam
- Ethernet
## What doesnt Work

- dGPU (1650 ti is unsupported in OC)
- HDMI (connected to the dGPU)
- Bluetooth
- AirDrop
- Headphone Jack (Untested)

## Photos

![Image 1](/img/1.jpeg)
![Image 2](/img/2.jpeg)
![Image 3](/img/3.jpeg)
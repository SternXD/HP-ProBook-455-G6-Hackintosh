# HP ProBook 455 G6 Hackintosh

## Configuration

| Specifications      | Detail                       |
| ------------------- | ---------------------------- |
| CPU                 | AMD Ryzen 3 2200U   |
| Integrated Graphics | AMD Vega 3       |
| Sound Card          | Realtek ALC236 (layout-id:3) |
❌ | Wireless Card       | External USB Dongle               |

## MacOS Versions Supported:

- macOS Sonoma
- macOS Ventura
- macOS Monterey
- macOS Big Sur
- macOS Catalina

## Changelog

### 10/31/2023

#### Preliminary release 

## What is Working?

- [x] Native CPU Power Management
- [x] Sleep/Wake
- [x] Intel Graphics
- [x] Audio
- [x] Trackpad (gestures)
- [x] Type-C USB
- [x] Type-C: video and audio
- [x] HDMI: video and audio
- [x] USB 3.0
- [x] Battery Management (thanks to [anor4k](https://www.tonymacx86.com/threads/guide-how-to-patch-dsdt-for-working-battery-status.116102/page-500#post-2021126) and [e285ne](https://www.tonymacx86.com/threads/guide-hp-probook-430-g6-whiskey-lake.282302/page-6#post-2147595))
- [x] Brightness
- [x] Brightness fn keys (if not working, turn off the laptop and hold the power button for 30 seconds to reset EC)
- [x] Built-in camera
- [x] Built-in mic
- [x] Line-in mic
- [x] Bluetooth Intel
- [x] Intel wireless
- [x] Fn keys: play/pause, prt scr(F13), sound mute/-/+, sleep

## Not working:

- [ ] Fingerprint reader
- [ ] SD Card Reader

## BIOS settings

- [ ] Fast Boot
- Secure Boot Configurations - Configure Legacy Support and Secure Boot = Legacy Support Disable and Secure Boot Disable
- [ ] VTx in System Options
- Wake On LAN = Disabled
- Wake On WLAN = Disabled
- Video Memory size = 64 MB
- [ ] Fingerprint Device
- [ ] Media Card Reader in Port Options
- Wake on USB = optional

## For 440/450 users:

- Disable **USBPorts.kext** and remap USB with **USBInjectAll.kext** using **[Dortania guide](https://dortania.github.io/OpenCore-Post-Install/usb/intel-mapping/intel.html)** or **[Hackintool](https://www.tonymacx86.com/threads/release-hackintool-v3-x-x.254559/)**.
- Possibly need change layout-id in boot-args for **AppleALC.kext**

## IMPORTANT

Make sure to add SMBIOS of MacBook Pro 15.2 and serial number in config.plis.

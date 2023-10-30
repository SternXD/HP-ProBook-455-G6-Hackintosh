# HP ProBook 455 G6 Hackintosh

## Configuration

| Specifications      | Detail                       |
| ------------------- | ---------------------------- |
| CPU                 | AMD Ryzen 3 2200U   |
| Integrated Graphics | AMD Vega 3       |
| Sound Card          | Realtek ALC236 (layout-id:3) |
| ❌ Wireless Card    | External USB Dongle               |

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
- [x] AMD Graphics
- [] Audio
- [] Trackpad (gestures)
- [x] Type-C USB
- [] Type-C: video and audio **Cannot test**
- [x] HDMI: video and audio
- [x] USB 3.0
- [] Battery Management
- [x] Brightness
- [x] Brightness fn keys (if not working, turn off the laptop and hold the power button for 30 seconds to reset EC)
- [x] Built-in camera
- [x] Built-in mic
- [x] Line-in mic
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

## IMPORTANT

Make sure to add SMBIOS of MacBook Pro 16,3 and serial number in config.plist.

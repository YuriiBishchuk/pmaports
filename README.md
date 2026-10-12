# postmarketOS port for Google Pixel 4a (5G) (google-bramble)

This repository contains the downstream device and kernel packages for **Google Pixel 4a (5G)** (`google-bramble`), bringing full postmarketOS support with Phosh, multi-touch input, display scaling, and Wi-Fi.

## Directory Structure
- `device/downstream/device-google-bramble`: Device package (DTB, udev rules, display profiles, LD_PRELOAD DRM/statx hook, systemd environment drop-ins, phoc.ini)
- `device/downstream/linux-google-bramble`: Linux kernel 4.19 downstream package with monolithic display/input drivers and qcacld-3.0 Wi-Fi module

## Hardware Support Status
- **Booting**: Working (Fastboot Header v3)
- **Display**: Working (1080x2340 60Hz AMOLED via MSM DRM + Pixman software rasterizer)
- **Touchscreen**: Working (10-point capacitive multi-touch via FocalTech FT5446)
- **UI Scaling**: 2.75x configured in Phoc/Phosh
- **Wi-Fi**: Working (2.4 GHz & 5 GHz WPA2/WPA3 via NetworkManager)
- **Battery**: Working (UPower battery percentage and status)
- **USB Networking**: Working (NCM gadget with SSH access)

## Official postmarketOS Integration
Target upstream repository: [postmarketOS / pmaports](https://gitlab.postmarketos.org/postmarketOS/pmaports)
Branch: `device/google-bramble`

# Flagma OS

**Version:** 4.7.3 (Stable)  
**Release Date:** 09.12.2025 (18:34:50)

---

## Overview

**Flagma OS** is a stable operating system for Raspberry Pi 5 which is **based on Android 16**, designed with reliability, security, and updatability in mind. It features a modern kernel and optimized partition images (`system`, `vendor`, and `boot`) for maximum performance. 


### Install

Download [**Balena Etcher**](https://etcher.balena.io/#download-etcher), then download the installer on Windows. On Linux, open the executable file ./balena-etcher or AppImage (if x86, then sudo chmod +x balena-etcher.AppImage and also ./balena-etcher.AppImage). Then download the .zip archive with the image (available in the latest release's attached files). Unzip the .zip archive and extract the .img image. In **Balena Etcher**, select this image and a disk of 32 GB or more (low free space = system crash if saving data + unzipping the compressed image to disk). Click "Flash", which will install the image to a disk that can be installed on a Raspberry Pi 5.

#### Why can't everything be done simply using Raspberry Pi Imager?

> Raspberry Pi Imager requires strict adherence to the FAT structure, which is impossible with AOSP Android 16, as it has an ext system, and Raspberry Pi Imager will reject 99% of image validation, forcing you to format it. But with Balena Etcher, it doesn't strictly check FAT and will boot correctly even with an ext system, and everything will work.

---

## Key Features

- Enhanced support for touch input devices  
- Optimized file system for speed and stability  
- Flexible update structure via `system.img`, `vendor.img`, and `boot.img`  
- Full compatibility with existing Flagma OS applications
- **OTA updates are supported**
- There is a large community and developers who will always help with the problem.  

---

## Current Release

**Flagma OS 4.7.3 Stable Release**  

**Changes:**  
- Sensor update  
- Bug fixes

---

## Included Components

- `system.img` — the main system partition containing the OS kernel, libraries, and system applications  
- `vendor.img` — vendor partition with drivers, configurations, and additional software  
- `boot.img` — boot image for system initialization  

---

## License

This project is licensed under the New BSD 3-Clause License. See [LICENSE](LICENSE) for details.

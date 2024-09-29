
# Dell Latitude 5290 OpenCore EFI
## Overview

This EFI has been tested on Mac OS 13 `Ventura` Mac OS 14 `Sonoma` and Mac OS 15 `Sequoia`.


## Specs

| Part             | Description                                                                                                    |
| ---------------- | -------------------------------------------------------------------------------------------------------------- |
| CPU              | Intel® Core™ i3-8130u Processor (will most likely work on core i5/i7 variants too)                             |
| iGPU             | Intel® HD 620     (Guide to give 64mb of VRAM found [here](https://github.com/lukeshondas/Dell-Latitude-5290-Opencore/blob/main/Update%20bios%20to%2064MB.md))  |
| Memory           | 32Gb (2 x 16Gb 2400MHz) (should work fine with 8gb+)                                                           |
| Storage          | SSD 512gb NVMe (should work fine with SATA SSD's too)                                                          |
| Display          | 12.5 inch <s>1366x768 TN Panel</s> 1920x1080 IPS Matte Panel (CONFIRMED A 1080p Panel works in this machine!)     |
| Wifi & Bluetooth | <s>Intel® Dual-Band Wireless-AC 8265</s> Dell DW1560 BCM94352Z                                                                              |
| LAN              | Intel® Gigabit Ethernet, 10/100/1000                                                                           |
| Audio            | Realtek ALC295                                                                                                 |
| External ports   | 1 x USB Type C, 2 x USB 3.0, 1 x Ethernet, 1 x Micro SD Card Reader, 1 x HDMI 1.4, 1 x 3.5 headphone/microphone combo, 1 x VGA |

### Working and Not Working

|                                                   | Status | Note                              |
| ------------------------------------------------- | ------ | ----------------------------------|
| Keyboard (with volume keys, , media control keys) | ✅     |                                   |
| Touchpad with all gestures and buttons            | ✅     |                                   |
| Ethernet                                          | ✅     |                                   |
| Wifi                                              | ✅     |Intel only with [Heliport](https://github.com/OpenIntelWireless/HeliPort) on Sequoia and Ventura|
| Bluetooth                                         | ✅     |Fixed!                             |
| SD Card Reader                                    | ✅     |                                   |
| Camera & Mic                                      | ✅     |                                   |
| Speaker & 3.5mm audio port                        | ✅     |Speaker working fine but audio jack is distorted (might be specific to my machine) |
| iGPU & VGA & HDMI                                 | ✅     |USB-C display output working unless monitor is higher resoultion than 1080p [Help?](https://www.reddit.com/r/hackintosh/comments/1fkvzgb/needing_help_with_a_weird_gpu_issue_i_just_cannot/)|
| USB                                               | ✅     |                                   |
| Sleep                                             | ✅     |                                   |
| Handoff                                           | ✅     |                                   |
| Airdrop                                           | ❌/✅  |Working with DW1560                |


## Usage

Download my EFI, Change your Serial with [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and install.

If installing Sequoia or Ventura and using Intel wifi you'll need to download [Heliport](https://github.com/OpenIntelWireless/HeliPort)

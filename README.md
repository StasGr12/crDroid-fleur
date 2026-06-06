# crDroid Fleur Releases

**Before you install the ROM**

**Please NOTE that I am new in custom rom development and might not provide excellent support for the ROM**

**If you encounter any issue please open github issue!**

## Device Sources
| Type  | Source | Revision |
|----|----|----|
| Device | [mt6781-devs/android_device_xiaomi_fleur](https://github.com/mt6781-devs/android_device_xiaomi_fleur) | lineage-23.2 |
| Vendor | [z3rh0/proprietary_vendor_xiaomi_fleur](https://github.com/z3rh0/proprietary_vendor_xiaomi_fleur) | lineage-23.2 |
| Kernel | [mt6781-devs/android_kernel_xiaomi_mt6781](https://github.com/mt6781-devs/android_kernel_xiaomi_mt6781) | lineage-23.2 |

# Instructions:
## Flashing Instuctions
Before installing please remember that:

**YOU are choosing to make these modifications and**

**I am not responsible for bricked devices or dead SD cards**
### Prequirements:
- Unlocked Bootloader
### Flashing Instructions:
 1. Download and install:
   - [ADB & FASTBOOT](https://developer.android.com/tools/releases/platform-tools?hl=en)
   - [Google USB Drivers](https://developer.android.com/studio/run/win-usb?hl=en)
 2. Reboot the PC
 3. Download the ROM ZIP and boot.img from [releases](https://github.com/StasGr12/crDroid-fleur/releases) and move them to the directory with ADB & FASTBOOT
 4. Flash the boot.img and reboot to recovery:
    - Enter the directory with ADB & FASTBOOT from CMD using cd command
    - Hold power button and volume down until the screen shows FASTBOOT
    - Plug your phone to your PC via USB and run fastboot devices in the CMD
      - If it shows a device your good to go
    - Flash the boot.img
      - Run this commands in CMD:
      - fastboot flash boot_a boot.img
      - fastboot flash boot_b boot.img
    - Reboot to recovery
      - Run this command in CMD:
      - fastboot reboot recovery
 5. Install the ROM
    - When in recovery press the Factory Reset button then press format data twice
    - Press apply update button and Apply from ADB
    - Run this command in CMD:
    - adb sideload <ROM NAME>.zip
    - Make sure that you replace <ROM NAME> with the real name of ROM zip file
    - Press the reboot to system button
 6. Enjoy!

## Device specifications

|                   Basic | Spec Sheet                                                         |
| ----------------------: | :----------------------------------------------------------------- |
|                     SoC | MediaTek® Helio G96 (MT6781)                                       |
|                     CPU | Octa-core CPU with 2x Cortex-A76 & 6x Cortex-A55                   |
|                     GPU | Mali-G57 MC2                                                       |
|                  Memory | 6/8 RAM (LPDDR4X)                                                  |
| Shipped Android Version | 11 with MIUI 13                                                    |
|                 Storage | 64/128/256 (UFS 2.2)                                               |
|                 Battery | 5000 mAh, non-removable                                            |
|                 Display | 1080 x 2400 pixels, 20:9 ratio, 6.43 inches, 60/90 Hz, AMOLED      |
|                  Camera | 108MP/64MP (Primary), 8MP (Ultra-wide), 2MP (Macro)                |

![Redmi Note 11S](https://i01.appmifile.com/v1/MI_18455B3E4DA706226CF7535A58E875F0267/pms_1678377190.61589211!800x800!85.png)

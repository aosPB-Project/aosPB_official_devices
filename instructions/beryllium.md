# Flashing instructions for Xiaomi POCO F1 (beryllium)

## Clean Flash (coming from a different ROM)
Clean flash involves formatting data which means you will be loosing data stored in the internal storage of your device, data in SD Card should not be affected. We will not be responsible for any loss of data.

1. Download ROM, recovery and super_empty files to your computer
2. Reboot the device to bootloader (Fastboot Mode)
3. Flash empty super image by running `fastboot wipe-super path/to/super_empty.img` in terminal
4. Flash recovery image by running `fastboot flash recovery path/to/recovery.img` in terminal
5. Reboot to recovery mode by holding volume up + power button
6. Go to main menu > Factory reset > Format Data > click "Format data" to confirm 
7. Similarly Format cache and system Partitions
8. Go to Apply update > Enable ADB Sideload
9. Flash the latest MIUI firmware for your region [POCO F1 / Pocophone F1 - Beryllium][def-beryllium] through ADB sideload by running `adb sideload path/to/firmware.zip`
10. Flash the ROM through ADB sideload by running `adb sideload path/to/rom.zip` in terminal
11. Reboot and voila!

## Dirty Flash / Update
There will be no loss of data if everything goes well. Keep backups incase of any mishap. I will not be responsible for any loss of data.

1. Download ROM file to your computer
2. Reboot the device to recovery
3. On your phone [which is in recovery mode], Apply update > Apply from ADB
4. Flash the ROM through ADB sideload by running `adb sideload path/to/rom.zip` in terminal
5. Reboot and voila!

[def-beryllium]: https://xmfirmwareupdater.com/firmware/beryllium/stable/V12.0.3.0.QEJMIXM/
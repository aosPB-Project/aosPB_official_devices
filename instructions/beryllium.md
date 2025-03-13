# Flashing instructions for Xiaomi Poco F1 (beryllium)

## Clean Flash (coming from a different ROM)
Clean flash involves formatting data which means you will be loosing data stored in the internal storage of your device, data in SD Card should not be affected. I will not be responsible for any loss of data.

1. Download ROM, recovery and super_empty files to your computer (click on recovery button for recovery and super_empty)
2. Reboot the device to bootloader (Fastboot Mode)
3. Flash empty super image by running fastboot wipe-super `path/to/super_empty.img` in terminal
4. Flash recovery image by running fastboot flash recovery `path/to/recovery.img` in terminal
5. Reboot to recovery mode
6. Go to main menu > Factory reset > Format data/factory reset > Format data - Back to Main menu
7. On your phone [which is in recovery mode], Apply update > Apply from ADB
8. Flash the ROM through ADB sideload by running adb sideload `path/to/rom.zip` in terminal
9. Reboot and voila!

## Dirty Flash / Update
There will be no loss of data if everything goes well. Keep backups incase of any mishap. I will not be responsible for any loss of data.

1. Download ROM file to your computer
2. Reboot the device to recovery
3. On your phone [which is in recovery mode], Apply update > Apply from ADB
4. Flash the ROM through ADB sideload by running adb sideload `path/to/rom.zip` in terminal
5. Reboot and voila!
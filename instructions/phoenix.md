# Flashing instructions for Xiaomi Redmi K30 / POCO X2 (phoenix/phoenixin)

## Clean flash (coming from a different ROM):
Clean flash involves formatting data which means you will be loosing data stored in the internal storage of your device, data in SD Card should not be affected. I will not be responsible for any loss of data.

1. Download ROM and recovery files to your computer
2. Reboot the device to bootloader (Fastboot Mode)
3. Flash the recovery by running fastboot flash recovery `path/to/recovery.img` in terminal
4. Reboot to recovery by holding volume up + power button
5. Go to Advanced > Enable ADB Sideload
6. Flash the latest MIUI firmware for your region through ADB sideload by running adb sideload `path/to/firmware.zip`
7. Flash the ROM through ADB sideload by running adb sideload `path/to/rom.zip` in terminal
8. Go to main menu > Wipe > Format Data > Type "yes" and confirm
9. Reboot and voila!

## Dirty Flash / Update
There will be no loss of data if everything goes well. Keep backups incase of any mishap. I will not be responsible for any loss of data.

1. Download ROM file to your computer
2. Reboot the device to recovery
3. On your phone [which is in recovery mode], go to Advanced > Enable ADB Sideload
4. Flash the ROM through ADB sideload by running adb sideload `path/to/rom.zip` in terminal
5. Reboot and voila!
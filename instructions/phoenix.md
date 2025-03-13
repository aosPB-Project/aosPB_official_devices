# Flashing instructions for Xiaomi Redmi K30 / POCO X2 (phoenix/phoenixin)

## Clean flash (coming from a different ROM):
Clean flash involves formatting data which means you will be loosing data stored in the internal storage of your device, data in SD Card should not be affected. We will not be responsible for any loss of data.

1. Download ROM and recovery files to your computer
2. Reboot the device to bootloader (Fastboot Mode)
3. Flash the recovery by running `fastboot flash recovery path/to/recovery.img` in terminal
4. Reboot to recovery by holding volume up + power button
5. Go to main menu > Factory reset > Format Data > click "Format data" to confirm 
6. Similarly Format cache and system Partitions
7. Go to Apply update > Apply from ADB
8. Flash the latest MIUI firmware for your region [Redmi K30 4G - Phoenix][def-phoenix] / [POCO X2 - Phoenixin][def-phoenixin] through ADB sideload by running `adb sideload path/to/firmware.zip`
9. Flash the ROM through ADB sideload by running `adb sideload path/to/rom.zip` in terminal 
10. Reboot and voila!

## Dirty Flash / Update
There will be no loss of data if everything goes well. Keep backups incase of any mishap. I will not be responsible for any loss of data.

1. Download ROM file to your computer
2. Reboot the device to recovery
3. On your phone [which is in recovery mode], go to Apply update > Apply from ADB
4. Flash the ROM through ADB sideload by running `adb sideload path/to/rom.zip` in terminal
5. Reboot and voila!

[def-phoenix]: https://xmfirmwareupdater.com/firmware/phoenix/stable/V13.0.6.0.SGHCNXM/

[def-phoenixin]: https://xmfirmwareupdater.com/firmware/phoenixin/stable/V12.5.7.0.RGHINXM/
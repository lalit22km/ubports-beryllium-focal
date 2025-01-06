# ubports-beryllium-focal
Unofficial janky setup to use Ubuntu Touch 20.04 Focal on Xiaomi Poco F1 (beryllium)

**Sources**
https://gitlab.com/joelselvaraj/xiaomi-beryllium/-/artifacts
https://github.com/ubports/installer-configs/blob/master/v2/devices/beryllium.yml

# Install Instructions
You can manually download all the files or download the zip in the release.
I'm assuming you already have an unlocked bootloader and have TWRP installed.

- Flash the firmware.zip using TWRP
- Reboot to bootloader/fastboot
- Flash the images
```
fastboot flash boot boot.img
fastboot flash recovery recovery.img
fastboot flash vendor vendor.img
fastboot flash system system.img
# Reboot
fastboot reboot
```
Avoid rebooting using power button. Use fastboot reboot.

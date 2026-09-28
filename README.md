# Mageia-iso-boot-support
Directly boot & install Mageia from Official Mageia Installation Media using grub2 without burning to usb-drive.

# Features
- Filesystems: exfat, ext4
- Provide Mageia boot menu
- Supported ISOs: Mageia-Live-iso files of Mageia-9/10 release.

# Usage
Load provided 'mageia-10.img' along with the main 'initrd' of the installation media via grub loopback module.
If you are using 'https://github.com/Mexit/MultiOS-USB', it is just a few steps:

0. Use MultiOS-USB partition on 'exfat' or 'ext4' filesystem.
1. Copy your Mageia iso files to 'ISOs' directory.
2. Create a directory for 'grub.cfg' files: '/MultiOS-USB/config_priv/Mageia-scandev'
3. Copy 'mageia-10.img' & 'Mageia-10-live.cfg' over there.
4. Reboot into 'MultiOS-USB' and start e.g. 'Mageia-10-Live-Plasma-x86_64.iso [scandev]' entry.
5. Live system should start same way as from a usb-stick.

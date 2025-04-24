# Ubuntu

## Installation
1. Download the distro.release.iso
2. Install either balenaEtcher or Rufus
3. Flash the iso onto a >16 GB USB sticker to make it bootable
4. Restart and boot from USB (access BIOS and reorder the boot order)
5. Follow the setup instructions
6. Come pre-installed: Python3, FDisk, man, Parted, tar, Vim, ssh

## Post-install
1. Remove all the bloat; some of them (thunderbird, rhytmbox, firefox etc...) can be removed via terminal
```bash
sudo apt list --install
sudo apt remove thunderbird
```
others have to be removed via Ubuntu Software (i.e. snap) which has therefore to be uninstalled last. Once done do
```bash
sudo apt autoremove
sudo apt purge
```
and then restart!
2. Update 
```bash 
sudo apt update
sudo apt upgrade
```
3. Install dev tools (approx 500 MB)
- [] gcc
- [] make
- [] CMake
- [] Git
- [] htop
- [] neofetch
- [] onefetch
then do
```bash
sudo apt purge --auto-remove
```
and restart!

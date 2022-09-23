# Arch Easy Install


- use `archinstall`
- chroot in to the system
- use the command `systemctl disable fstrim.timer`


# Install Graphic Driver
```
su username
mkdir ~/pkgs
cd ~/pkgs
git clone https://aur.archlinux.org/yay.git
cd yay
sudo pacman -S xorg-server linux-headers
makepkg -si
yay -S nvidia-390xx
```

# Install Desktop
```
sudo pacman -S plasma kde-applications discord firefox
sudo systemctl enable sddm
```

# common things that might help ya because it helped me lot while using arch linux with hyprland in my day to day life.

## To open dolphin file manager as root

```bash
su -c dolphin
```

## To Change Cursor in Hyprland

```bash
hyprctl setcursor cursorname cursorsize
                  ^^         ^^
```

## To install Vencord

```bash
sh -c "$(curl -sS https://raw.githubusercontent.com/Vendicated/VencordInstaller/main/install.sh)"
```

## To mount a ntfs partition (sudo) dependency: ftfs-3g
```bash
mount -o rw -t ntfs-3g /dev/nvmexxxxx ~/Destination/
```

## To update pacman mirror
```bash
sudo reflector --verbose --latest 10 --sort rate  --download-timeout 20 --save /etc/pacman.d/mirrorlist
```

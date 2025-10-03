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

## To mount a ntfs partition 
```bash
mount -o rw -t ntfs-3g /dev/nvmexxxxx ~/Destination/
```
dependency: ntfs-3g


## To update pacman mirror
```bash
sudo reflector --verbose --latest 10 --sort rate  --download-timeout 20 --save /etc/pacman.d/mirrorlist
```

## Single line command that can run any music video from youtube silently in the background. 
```bash
yt-dlp -f bestaudio ytsearch:"Let the world burn - Chris Grey" -o - 2>/dev/null | ffplay -nodisp -autoexit -i - &>/dev/null
```
dependency: ffplay yt-dlp


## To Zip a folder.
```bash
zip -r archive_name.zip folder_to_zip/
```
dependency: zip

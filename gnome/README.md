#load gnome backup
dconf load / < gnome-full-backup.txt

#load only keybinds
dconf load /org/gnome/desktop/wm/keybindings/ < gnome-keybindings-backup.txt
dconf load /org/gnome/settings-daemon/plugins/media-keys/ < gnome-custom-keybindings-backup.txt

#create gnome backup
dconf dump / > gnome-full-backup.txt

#create only keybinds backup
dconf dump /org/gnome/desktop/wm/keybindings/ > gnome-keybindings-backup.txt
dconf dump /org/gnome/settings-daemon/plugins/media-keys/ > gnome-custom-keybindings-backup.txt


# Get along with GNOME
### Add this lines to your `~/.config/i3/config`:

### GNOME Settings Daemon
```
exec --no-startup-id /usr/lib/gnome-settings-daemon/gsd-xsettings
```
[gsd-xsettings](https://bugs.archlinux.org/task/53800).

### GNOME power manager
```
exec_always --no-startup-id gnome-power-manager
```

### polkit-gnome 
```
exec --no-startup-id /usr/lib/polkit-gnome/polkit-gnome-authentication-agent-1
```
Starts authentication-agent needed to get `sudo` password check aviable for GUIs needing it.
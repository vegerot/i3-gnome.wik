# get along with GNOME
Add this lines to your `~/.config/i3/config`:
```
exec --no-startup-id /usr/lib/gnome-settings-daemon/gsd-xsettings
exec_always --no-startup-id gnome-power-manager
```
And you'll have more integration about `GNOME Settings Daemon` and GNOME power manager.
More about `gsd-xsettings` [here](https://bugs.archlinux.org/task/53800).
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
Starts authentication-agent needed to get `sudo` password check available for GUIs needing it.

### [GNOME Flashback](https://wiki.gnome.org/Projects/GnomeFlashback)
```
exec --no-startup-id gnome-flashback
```
GNOME Flashback integrates more features from GNOME such as full functionality for `gnome-control-center`:
> Gnome-flashback is specifically designed to recover some functionality already moved to mutter or gnome-shell. 
> So, it comes with some features built in but easy to disable if you want to.

Also it helps with function keys including bright screen management, sound and so on **out-of-the-box**.

Note: this approach (finally) fixes [#11](https://github.com/jcstr/i3-gnome/issues/11) in a simple way.

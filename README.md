# Flatpak permission cleaner
Overwrite the storage permissions of all flatpaks that have host-permissions with something that actually makes sense.

Many Flatpaks, especially popular ones like GIMP, Libreoffice e.g. can access all your files and break everything. They may not do that, but this is not what security looks like. This tool easily allows you to change that.

By default that is:

- `$HOME`
- `/run/media/$USER`
- `/mnt`
- `/var/mnt`
- `mtp:`

You have the option to set different filesystems though, just enter your locations, seperated by a space.

Install:

```
wget https://github.com/trytomakeyouprivate/flatpak-permission-cleaner/raw/main/flatpak-permission-cleaner -P ~/.local/bin
chmod +x ~/.local/bin/flatpak-permission-cleaner
```

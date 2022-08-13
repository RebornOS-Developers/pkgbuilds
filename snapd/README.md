# snapd

Service and tools for management of snap packages.

**WARNING**: If you get the error message ***Unable to run aclocal***, install ***automake***:

```
sudo pacman -S automake
```

**NOTES:**
2.36 is the first release with AppArmor enabled by default on Arch.

If you do not have AppArmor enabled at boot there should be no functional changes visible.

If you wish to use snaps with Apparmor, first make sure that Apparmor is enabled during boot, see https://wiki.archlinux.org/index.php/AppArmor for details. After upgrading the package, you need to do the following steps:

Reload the profiles:
```
systemctl restart apparmor.service
```

Restart snapd:
```
systemctl restart snapd.service
```

Load profiles for snaps:
```
systemctl enable --now snapd.apparmor.service
```

https://github.com/snapcore/snapd

PKGBUILD in https://github.com/snapcore/snapd/tree/master/packaging/arch (this don't work)

To clone this repo:

```
git clone https://gitlab.com/rebornos-team/rebornos-packages/snapd.git
```

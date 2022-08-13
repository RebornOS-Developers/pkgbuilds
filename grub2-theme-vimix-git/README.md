# grub2-theme-vimix-git

RebornOS Grub2 theme Vimix

How to clone this repo:

```
git clone https://gitlab.com/reborn-os-team/rebornos-packages/grub2-theme-vimix-git.git
```


# If the following error occurs:

grub2-theme-vimix-git/PKGBUILD: line 37: cd: /var/tmp/pamac-build-[username]/grub2-theme-vimix-git/src/grub2-theme-vimix-git/assets/assets-white/select: No such file or directory

==> ERROR: A failure occurred in package().

# Solution:

Edit the file PKGBUILD and edit/modify line 37 to:

cd "${srcdir}/${pkgname}/assets/assets-white/select-1080p/"

or:

cd "${srcdir}/${pkgname}/assets/assets-white/select-2k/" or cd "${srcdir}/${pkgname}/assets/assets-white/select-4k/"


# This PKGBUILD is corrected with the first option.
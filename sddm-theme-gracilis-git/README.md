# sddm-theme-gracilis-git

Gracilis Theme for SDDM by mikkeloscar

https://github.com/mikkeloscar/sddm-gracilis-theme

How to clone this repo:

```
git clone https://gitlab.com/reborn-os-team/rebornos-packages/sddm-theme-gracilis-git.git
```

Original content of PKGBUILD:

```
# Maintainer: Emil Lundberg <emil@emlun.se>

pkgname=sddm-theme-gracilis-git
pkgver=latest
pkgrel=2
pkgdesc="Gracilis Theme for SDDM by mikkeloscar"
arch=('any')
url="https://github.com/mikkeloscar/sddm-gracilis-theme"
license=('CCPL:cc-by-sa')
depends=('sddm')
_theme_name='gracilis'
_repo_name='sddm-gracilis-theme'
source=("git+https://github.com/mikkeloscar/sddm-gracilis-theme.git")
md5sums=('SKIP')

pkgver() {
  echo "$(git -C "${srcdir}/${_repo_name}" rev-list --count HEAD).0.0"
}

package() {
  install -d "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}"
  cp -r "${srcdir}/${_repo_name}"/* "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}"/
  find "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}" -type d -exec chmod 555 {} \;
  find "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}" -type f -exec chmod 444 {} \;
}
```


Modified to RebornOS:

```
# Maintainer: Emil Lundberg <emil@emlun.se>

pkgname=sddm-theme-gracilis-git
pkgver=8.0.1
pkgrel=1
pkgdesc="Gracilis Theme for SDDM by mikkeloscar"
arch=('any')
url="https://github.com/mikkeloscar/sddm-gracilis-theme"
license=('CCPL:cc-by-sa')
depends=('sddm')
_theme_name='gracilis'
_repo_name='sddm-gracilis-theme'
source=("git+https://github.com/mikkeloscar/sddm-gracilis-theme.git")
md5sums=('SKIP')


package() {
  install -d "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}"
  cp -r "${srcdir}/${_repo_name}"/* "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}"/
  find "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}" -type d -exec chmod 555 {} \;
  find "${pkgdir}"/usr/share/sddm/themes/"${_theme_name}" -type f -exec chmod 444 {} \;
}
```


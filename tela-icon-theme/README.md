# tela-icon-theme

A flat colorful Design icon theme

https://github.com/vinceliuice/Tela-icon-theme

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/themes-and-icons/tela-icon-theme.git
```

<br>
PKGBUILD:

```
# Maintainer: Rafael <rafael@rebornos.org>

pkgname=tela-icon-theme
_pkgname=Tela-icon-theme
pkgver=2021.01.21
_pkgver=2021-01-21
pkgrel=1
pkgdesc="A flat colorful Design icon theme"
arch=('any')
url="https://github.com/vinceliuice/Tela-icon-theme"
license=('GPL3')
depends=('gtk-update-icon-cache')
options=('!strip')

source=("${url}/archive/refs/tags/${_pkgver}.tar.gz")
sha512sums=('ab2b7b1a7fdca3acf0e9dbf948a8ea88df0c3d77469df6bf3330c3ab2d480b4ebd203046a1a344aa5cfe51a2f7a2dd16bba4d8b29e5f903669e37601a9cee8f5')

package() {
    cd ${srcdir}/${_pkgname}-${_pkgver}
    install -m755 -d ${pkgdir}/usr/share/icons
    ./install.sh  -d ${pkgdir}/usr/share/icons
}
```

PKGBUILD 2:

```
# Maintainer: Rafael <rafael@rebornos.org>

pkgname=tela-icon-theme
_pkgname=Tela-icon-theme
pkgver=2021.01.21
commitn=f78ed967abe90ff1693f0a106d9a83f5c9565a1b
_pkgver=2021-01-21
pkgrel=1.1
pkgdesc="A flat colorful Design icon theme"
arch=('any')
url="https://github.com/vinceliuice/Tela-icon-theme"
license=('GPL3')
depends=('gtk-update-icon-cache')
options=('!strip')

source=("git+${url}#commit=${commitn}")
sha512sums=('SKIP')

package() {
    cd ${srcdir}/${_pkgname}
    install -m755 -d ${pkgdir}/usr/share/icons
    ./install.sh  -d ${pkgdir}/usr/share/icons
}
```



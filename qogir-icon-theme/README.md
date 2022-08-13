# qogir-icon-theme

A flat colorful design icon theme for linux desktops

https://github.com/vinceliuice/Qogir-icon-theme

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/themes-and-icons/qogir-icon-theme.git
```

PKGBUILD for version:

```
pkgname=qogir-icon-theme
_pkgname=Qogir-icon-theme
pkgver=2020.11.22
_pkgver=2020-11-22
pkgrel=1
pkgdesc="A colorful design icon theme for linux desktops"
arch=('any')
url="https://www.pling.com/p/1279924"
license=('GPL3')
depends=('hicolor-icon-theme' 'gtk-update-icon-cache')
options=('!strip')
source=("$pkgname-$pkgver.tar.gz::https://github.com/vinceliuice/$_pkgname/archive/$_pkgver.tar.gz")
sha256sums=('SKIP')

package() {
	cd "$_pkgname-$_pkgver"
	install -d "$pkgdir/usr/share/icons"
	./install.sh -d "$pkgdir/usr/share/icons"
}
```
Other PKGBUILD:

```
# Maintainer: Aitor Alonso <contact: https://aalonso.eu>


_pkgname=Qogir-icon-theme
_pkgver=2021-10-14
pkgname=qogir-icon-theme
pkgver=${_pkgver//-/.}
pkgrel=1
pkgdesc="A colorful design icon theme for linux desktops"
arch=('any')
url="https://github.com/vinceliuice/Qogir-icon-theme"
license=('GPL3')
depends=('hicolor-icon-theme' 'gtk-update-icon-cache')
options=('!strip')
source=("$pkgname-$pkgver.tar.gz::https://github.com/vinceliuice/$_pkgname/archive/$_pkgver.tar.gz")
sha256sums=('329032fb3a4e3d68a697dbea7fd4389a138c1da55a7433a1dc25803bda568d32')

package() {
	cd "$_pkgname-$_pkgver"
	install -d "$pkgdir/usr/share/icons"
	./install.sh -d "$pkgdir/usr/share/icons"
}
```



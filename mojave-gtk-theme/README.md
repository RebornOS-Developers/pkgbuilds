# mojave-gtk-theme

A Mac OSX like theme for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments like Gnome, Pantheon, XFCE, Mate, etc.

https://github.com/vinceliuice/Mojave-gtk-theme

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/themes-and-icons/mojave-gtk-theme.git
```

PKGBUILD:

```
# Maintainer: Rafael from RebornOS

pkgname=mojave-gtk-theme
_pkgname=Mojave-gtk-theme
pkgver=2021.07.20
_pkgver=2021-07-20
pkgrel=1
pkgdesc='Mac OSX like theme for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments.'
arch=('any')
url='https://github.com/vinceliuice/Mojave-gtk-theme'
license=('GPL3')
makedepends=('gdk-pixbuf2' 'glib2' 'sassc')
optdepends=('gtk-engine-murrine: GTK2 theme engine')
conflicts=('mojave-gtk-theme-git')
provides=("${pkgname}-${pkgver}")
source=("${url}/archive/refs/tags/${_pkgver}.tar.gz")
sha512sums=('be85934cfb123e2c5a015cb60b5665946b83d1f368e5c04cb41ef77b7141e500200f30b8e5bca76a2af9fceb5a9ac541d805c549d9b412f77bfe296ca0994869')

package() {
	cd "${srcdir}/${_pkgname}-${_pkgver}"
	install -m755 -d "${pkgdir}/usr/share/themes"
	./install.sh \
		 --dest "${pkgdir}/usr/share/themes" \
		 --icon arch
        find ${pkgdir}/usr -type f -exec chmod 644 {} \;
        find ${pkgdir}/usr -type d -exec chmod 755 {} \;
}
```


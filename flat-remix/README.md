# flat-remix

Flat remix is a pretty simple icon theme inspired on material design following a modern design using flat colors with high contrasts and sharp borders.

Home: https://github.com/daniruiz/flat-remix/

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/themes-and-icons/flat-remix.git
```
PKGBUILD for version:

```
# Maintainer: Daniel Ruiz de Alegria <daniruizdealegria@gmail.com>

pkgname="flat-remix"
pkgver=20210620
pkgrel=1
pkgdesc="Flat Remix is an icon theme inspired by material design. It is mostly flat using a colorful palette with some shadows, highlights, and gradients for some depth."
arch=('any')
url="https://drasite.com/flat-remix"
license=('GPL3')
options=('!strip')
source=("https://github.com/daniruiz/${pkgname}/archive/${pkgver}.tar.gz")
sha256sums=('SKIP')

package() {
	cd "${srcdir}/${pkgname}-${pkgver}/"
	make install DESTDIR=${pkgdir}
}
```



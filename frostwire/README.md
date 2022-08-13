# frostwire

Cloud Downloader, BitTorrent Client and Media Player

http://www.frostwire.com

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/rebornos-packages/frostwire.git
```

PKGBUILD ORIG:

```
# Maintainer: Manifest0
# Contributor: Dimitris Kiziridis <ragouel at outlook dot com>
# Contributor: Frederic Bezies <fredbezies at gmail dot com>
# Contributor: liberodark

pkgname=frostwire
pkgver=6.9.4
pkgrel=1
pkgdesc='Cloud Downloader, BitTorrent Client and Media Player'
arch=('x86_64')
url='http://www.frostwire.com'
license=('GPL')
depends=('hicolor-icon-theme' 'java-environment' 'bash' 'zlib')
optdepends=('mplayer: Media playback support')
source=("${pkgname}-${pkgver}.deb::https://prime.frostwire.com/frostwire/${pkgver}/frostwire-${pkgver}.amd64.deb")
sha256sums=('68f4638cdc43509ce025fb206d3dd019e29f7a0c15ae108815bf92189e2dcbc5')
 
package() {
  tar xvf data.tar.xz -C "${pkgdir}"
}
```


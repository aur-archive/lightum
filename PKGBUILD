# Maintainer: Luciano Ruete <lruete NOSPAM sequre.com.ar>


pkgname=lightum
pkgver=2.3.1
pkgrel=1
pkgdesc="MacBook automatic keyboard brightness daemon"
arch=('x86_64' 'i686')
url="https://github.com/poliva/lightum"
license=(GPL)
groups=()
depends=('dbus-glib' 'libxss' 'libx11' 'libxext')
makedepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=.install
changelog=
source=(https://github.com/poliva/$pkgname/tarball/v$pkgver)
noextract=()

build() {
  cd $srcdir/poliva-$pkgname-8326d25/
  make
}

package() {
  cd $srcdir/poliva-$pkgname-8326d25/
  make DESTDIR="$pkgdir" install
}

md5sums=('384a09646d7d500b1a5d8c84d609f536')

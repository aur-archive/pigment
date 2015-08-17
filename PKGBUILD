# Contributor: Stefan Husmann <stefan-husmann@t-online.de>
# Contributor: Andrea Scarpino <bash.lnx@gmail.com>
# Contributor: sickhate <sickhate@tux-linux.net>
# Contributor: Bjorn Lindeijer <bjorn lindeijer nl>

pkgname=pigment
pkgver=0.3.17
pkgrel=2
pkgdesc="A GLib/GObject library designed to easily create rich UIs embedding several media types"
arch=('i686' 'x86_64')
url="https://code.fluendo.com/pigment/trac"
license=('GPL')
depends=('libgl' 'gstreamer0.10-base' 'gtk2')
options=('!libtool')
source=(http://launchpad.net/pigment/0.3/0.3.17/+download/pigment-0.3.17.tar.bz2)
md5sums=('b0947a18cc9265f3129ff4b069c1ed0c')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  
  ./configure --prefix=/usr
  
  make || return 1
  make DESTDIR="$pkgdir" install
}
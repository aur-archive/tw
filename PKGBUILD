# Maintainer:  TDY <tdy@archlinux.info>
# Contributor: Dylon Edwards <deltaecho@archlinux.us>

pkgname=tw
pkgver=0.9.4
pkgrel=1
pkgdesc="Translate words into different languages"
url="http://code.google.com/p/translateword/"
license=('GPL')
arch=('any')
depends=('bash' 'curl' 'elinks' 'gawk' 'grep' 'libmythes' 'sed' 'util-linux-ng')
install=tw.install
source=(http://translateword.googlecode.com/files/tw-$pkgver.tar.bz2)
md5sums=('95ea0be3a831f00546de2be041c09264')

build() {
	cd "$srcdir/tw-$pkgver"
  ./configure --prefix=/usr
  make
}

package() {
	cd "$srcdir/tw-$pkgver"
  make DESTDIR="$pkgdir/" install
}

# vim:set ts=2 sw=2 et:

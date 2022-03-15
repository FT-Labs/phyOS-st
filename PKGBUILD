# Maintainer: Arda Atci<phystecharda@gmail.com>
pkgname=st-phyOS
pkgver=0.8.2
pkgrel=1
pkgdesc="st build for phyOS"
arch=(x86_64)
url="git://git.suckless.org/st"
license=('MIT')
depends=('libxft')
makedepends=('ncurses' 'libxext' 'git' 'make')
optdepends=('dmenu')
provides=("st")
conflicts=("st")
options=('zipman')
source=('git+https://github.com/PhyTech-R0/st-phyOS')
md5sums=('SKIP')

prepare() {
	cd $srcdir/${pkgname}
	sed -i '/tic /d' Makefile
}

build() {
	cd "$pkgname"
	make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11
}

package() {
	cd "$pkgname"
	make PREFIX=/usr DESTDIR="$pkgdir/" install
}

pkgname=beam-share
pkgver=1.0.2
pkgrel=1
arch=('i686' 'x86_64')
license=("GPL3")
source=()
depends=('nmap' 'fzf')

prepare() {
	ln -snf "$startdir" "$srcdir/$pkgname"
}

package() {
    cd "$pkgname"
    mkdir -p $pkgdir/usr/bin
    make DESTDIR="$pkgdir" install
}

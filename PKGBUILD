pkgname=m17n-db
pkgver=1.7.0
pkgrel=1
pkgdesc='Multilingual text processing library (database)'
url='http://www.nongnu.org/m17n/'
arch=('x86_64')
license=('GPL')
depends=('glibc')
source=("http://download.savannah.gnu.org/releases/m17n/${pkgname}-${pkgver}.tar.gz")
sha1sums=('4149c2e59ac8f45ec8cbfb7bc8d4d061f38e58bc')

build() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	./configure --prefix=/usr
	make
}

package() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make DESTDIR="${pkgdir}" install
}

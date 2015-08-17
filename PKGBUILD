# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-analytic-sale
_pkgname=trytond_analytic_sale
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The analytic_sale module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-analytic-account>=3.4' 'trytond-analytic-invoice>=3.4' 'trytond-sale>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("afcb5d3734c582194ddbb880738c4491")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}
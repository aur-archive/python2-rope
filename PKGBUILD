# $Id: PKGBUILD 64234 2012-02-11 00:28:07Z arodseth $
# Maintainer: Thomas Dziedzic < gostrc at gmail >
# Contributor: Nicolás de la torre <ndelatorre@gmail.com>
# Contributor: Ryan Coyner <rcoyner@gmail.com>
# Contributor: Jens Maucher <defcon@archlinux.us>

pkgname=python2-rope
pkgver=0.9.3
pkgrel=4
pkgdesc='A Python refactoring library'
arch=('any')
url='http://rope.sourceforge.net'
license=('GPL')
depends=('python2')
source=("http://pypi.python.org/packages/source/r/rope/rope-${pkgver}.tar.gz")
md5sums=('b04971636816d62157cf26e2ec5c1a37')

build() {
  cd rope-${pkgver}

  python2 setup.py build
}

package() {
  cd rope-${pkgver}

  python2 setup.py install --root=${pkgdir} --optimize=1
}

# Maintainer: jsteel <mail at jsteel dot org>
# Contributor: Anton Bazhenov <anton.bazhenov at gmail>

pkgname=python-rabbyt-old
pkgver=0.8.1
pkgrel=2
pkgdesc="A sprite library for Python with game development in mind (older version)"
arch=('i686' 'x86_64')
url="http://arcticpaint.com/projects/rabbyt"
license=('LGPL')
depends=('python2' 'mesa')
makedepends=('pyrex' 'setuptools')
provides=('python-rabbyt')
conflicts=('python-rabbyt')
source=(http://pypi.python.org/packages/source/R/Rabbyt/Rabbyt-$pkgver.tar.gz)
md5sums=('30c143d133a6abaf8ab2ba3516ae7fc2')

build() {
  cd "$srcdir"/Rabbyt-$pkgver

  python2 setup.py build
}

package() {
  cd "$srcdir"/Rabbyt-$pkgver

  python2 setup.py install --root="$pkgdir"
}

# Maintainer: Supun Adithya <contact@supunadithya.com>
pkgname=zapzap
pkgver=6.2.7
pkgrel=1
pkgdesc="WhatsApp Messenger for Linux"
arch=('any')
url="https://github.com/rafatosta/zapzap"
license=('GPL3')
depends=('python' 'python-pyqt6' 'python-pyqt6-webengine' 'dbus-python')
makedepends=('git' 'python-build' 'python-installer' 'python-wheel' 'python-setuptools')
source=("zapzap-src::git+file:///home/supun/projects/forks/zapzap")
md5sums=('SKIP')

pkgver() {
  cd "$srcdir/zapzap-src"
  # Try to extract version from __init__.py, fallback to hardcoded if needed
  _ver=$(grep -oP "__version__ = '\K[^']+" zapzap/__init__.py)
  if [ -n "$_ver" ]; then
    echo "$_ver"
  else
    echo "6.2.7"
  fi
}

build() {
  cd "$srcdir/zapzap-src"
  python -m build --wheel --no-isolation
}

package() {
  cd "$srcdir/zapzap-src"
  python -m installer --destdir="$pkgdir" dist/*.whl
}

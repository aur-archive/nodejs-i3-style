_npmname=i3-style
_npmver=0.4.0
pkgname=nodejs-i3-style # All lowercase
pkgver=0.4.0
pkgrel=1
pkgdesc="Make your i3wm config a little more stylish"
arch=(any)
url="https://github.com/acrisci/i3-style"
license=()
depends=('nodejs' )
optdepends=()
source=(http://registry.npmjs.org/$_npmname/-/$_npmname-$_npmver.tgz)
noextract=($_npmname-$_npmver.tgz)
sha1sums=(42d15dd9cbda83aece25cec8f2f430d0964a15d0)

package() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p $_npmdir
  cd $_npmdir
  npm install -g --prefix "$pkgdir/usr" $_npmname@$_npmver
}

# vim:set ts=2 sw=2 et:
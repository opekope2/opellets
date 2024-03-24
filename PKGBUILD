# Maintainer: opekope2 <opekope2@gmail.com>

_gitname=opellets
pkgname=$_gitname-git
pkgver=1
pkgrel=1
pkgdesc="Manage installed Arch packages with a configuration file"
arch=('any')
url="https://github.com/opekope2/$_gitname"
license=('Unlicense')
depends=('bash' 'sudo')
source=("git+https://github.com/opekope2/$_gitname")
sha256sums=('SKIP')

pkgver() {
	cd "$srcdir/$_gitname"
	echo "r$(git rev-list --count HEAD).$(git rev-parse --short HEAD)"
}

package() {
	cd "$srcdir/$_gitname"
	install -Dm775 "opellets" "$pkgdir/usr/bin/opellets"
}

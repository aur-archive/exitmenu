# Maintainer: trile7 at gmail dot com

pkgname=exitmenu
pkgver=0.2
pkgrel=4
pkgdesc="poweroff, reboot, logoff, sleep, and hibernate script that gracefully close windows before execution"
url="http://bashscripts.googlecode.com"
arch=('i686' 'x86_64')
license=('GPL3')
depends=(yad grep coreutils bash sudo wmctrl)
optdepends=("pm-utils: to sleep or hibernate")
install=$pkgname.install
source=($url/files/$pkgname-$pkgver.tar.gz)

package() {
  mkdir -p "$pkgdir/usr/share/$pkgname"
  mkdir -p "$pkgdir/usr/bin"
  cp "$srcdir/$pkgname-$pkgver"/* "$pkgdir/usr/share/$pkgname"
  mv "$pkgdir/usr/share/$pkgname/$pkgname" "$pkgdir/usr/bin"
}

md5sums=('305666cbf1017a96a653360355035d28')

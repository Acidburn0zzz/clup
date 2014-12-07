# Maintainer: Colin Keenan <colinnkeenan at gmail dot com>

pkgname=clup
pkgver=1.0
pkgrel=1
pkgdesc="Clickable/configurable Update of Arch Linux"
arch=('any')
url="https://github.com/colinkeenan/clup"
license=('GPL')
install=${pkgname}.install

source=(${pkgname} ${pkgname}.conf ${pkgname}.desktop)
md5sums=('ad23467d8c4860e5b53cbec8dc86756a'
         'f6cfb2a1085bbcf48b46471be30fcb89'
         '0abe59259a20e473417204c8f31543f9')

package() {
  install -D -m755 ${pkgname}.conf "$pkgdir/etc/${pkgname}.conf"
  install -D -m755 ${pkgname}.desktop "$pkgdir/usr/share/applications/${pkgname}.desktop"
  install -D -m755 ${pkgname} "$pkgdir/usr/bin/${pkgname}"
}

pkgname=2gis-ulyanovsk
pkgver=20
pkgrel=1
pkgdesc="Map of Ulyanovsk for 2GIS, July 2013"
arch=('i686' 'x86_64')
url="http://ulyanovsk.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Ulyanovsk-20.orig.zip")
md5sums=('83f29dad9b29d1100fc49ab56ea1d630')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Ulyanovsk.dgdat" "${pkgdir}/opt/2gis/ulyanovsk.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Ulyanovsk.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/ulyanovsk.dglf" || return 1
}

# Contributor: Krzysztof Raczkowski <raczkow@gnu-tech.pl>
# Maintainer: alexmo82 <25396682@live.it>

pkgname=kde-servicemenus-pdf
pkgver=0.6
pkgrel=2
pkgdesc="KDE service menus for PDF documents"
arch=('any')
url="http://kde-apps.org/content/show.php/KDE+Service+Menu+PDF?content=37321"
license=('GPL')
depends=('kdebase-workspace>=4.5.0' 'ghostscript' 'texlive-core' 'poppler' 'pdftk')
source=(http://kde-apps.org/CONTENT/content-files/37321-kde-service-menu-pdf_0.6.tar.gz)
md5sums=('ee032d4984b6eb91d77b33ed82632381')

package() {
  mkdir -p ${pkgdir}/usr/share/kde4/services/ServiceMenus/
  mkdir -p ${pkgdir}/usr/bin/
  install -m 644 ${srcdir}/kde-service-menu-pdf_$pkgver/desktop/*.desktop ${pkgdir}/usr/share/kde4/services/ServiceMenus/
  install -m 755 ${srcdir}/kde-service-menu-pdf_$pkgver/bin/* ${pkgdir}/usr/bin/
}

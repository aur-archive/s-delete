# Maintainer: Paolo Stivanin <admin@polslinux.it>
# Come to visit my site: http://www.polslinux.it

pkgname=s-delete
_pkgname=secure-delete
pkgver=1.12.0.1
pkgrel=2
pkgdesc="Perform secure files and folders deletion thanks to shred and wipe"
arch=('i686' 'x86_64')
url="https://github.com/polslinux/Secure-Delete"
license=('GPL')
depends=('yad' 'bash' 'curl' 'wipe' 'wget')
provides=('${pkgname}=${pkgver}')
source=(https://github.com/downloads/polslinux/Secure-Delete/${_pkgname}_v${pkgver}.tar.bz2)
md5sums=('972d9d6f1c5895cafb42543de03d7360')

build() {
  cd ${srcdir}
  mkdir -p ${pkgdir}/usr/local/bin
  mkdir -p ${pkgdir}/usr/share/doc/secure-delete
  cp bin/sdelete.sh ${pkgdir}/usr/local/bin/sdelete
  cp bin/sdelete_update.sh ${pkgdir}/usr/local/bin/sdelete_update
  mkdir ${pkgdir}/usr/share/doc/secure-delete && cp docs/* ${pkgdir}/usr/share/doc/secure-delete/
  cp LICENSE README.md uninstall ${pkgdir}/usr/share/doc/secure-delete/
}

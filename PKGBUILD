# Maintainer: Itsuki0222 <krypton@f5.si>

pkgname=kryptonlinux-keyring
pkgver=20250601
pkgrel=1
pkgdesc="Krypton Linux PGP keyring."
arch=(any)
install="${pkgname}.install"
url="https://krypton-linux.com/"
license=("MIT")

source=('https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/Makefile'
        'https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/kryptonlinux-trusted'
        'https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/kryptonlinux-revoked'
        'https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/kryptonlinux.gpg')

sha256sums=("SKIP")
validpgpkeys=("5384B7916710F361C29659BC3EFCB5A1E5F25C93") #Itsuki0222


package() {
    cd "${srcdir}"
    make PREFIX=/usr DESTDIR=${pkgdir} install
}

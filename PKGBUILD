# Maintainer: Itsuki0222 <krypton@f5.si>

pkgname=kryptonlinux-keyring
pkgver=20250601
pkgrel=1
pkgdesc="Krypton Linux PGP keyring."
arch=(any)
install="${pkgname}.install"
url="https://krypton-linux.com/"
license=("MIT")

source=('https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/main/Makefile'
        'https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/main/kryptonlinux-trusted'
        'https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/main/kryptonlinux-revoked'
        'https://raw.githubusercontent.com/krypton-linux/kryptonlinux-keyring/main/kryptonlinux.gpg')

sha256sums=('57fc188eb1eb81c6fd4ba98e795adf4a98f3e553c2b87afabbaf65cb5c1df22d'
            'bf6d3de49bad87e394f542cf19708356fdac19255315200bb089eb360426f735'
            'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'
            '9abe77dfb84802cc383768b5820b70a4ba4eab9ed42c460724d5ef913b2392fc')

validpgpkeys=("5384B7916710F361C29659BC3EFCB5A1E5F25C93") #Itsuki0222


package() {
    cd "${srcdir}"
    make PREFIX=/usr DESTDIR=${pkgdir} install
}

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

sha256sums=('f3bf64f5cee5e04679897c26c84ed3a5e3b22a0234fd07d8006e72ef9ede18bd'
            '78f0a9e679de6b8ec224d9bd8fb65f6f216c14d287e8ed0c59a08c0e65a93483'
            'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'
            '85a7fc3306002d409aab90432b30f3075e910fb1a18eaeafcf690121b606e6c2')

validpgpkeys=("5384B7916710F361C29659BC3EFCB5A1E5F25C93"  #Itsuki0222
              "4A23DFF9A4C7C7780EF378BAF6D88F90EF627755") #TNTSuperMan


package() {
    cd "${srcdir}"
    make PREFIX=/usr DESTDIR=${pkgdir} install
}

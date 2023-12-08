pkgname='nimaos-inst-git'
pkgver=r3.76d89ef
pkgrel=1
pkgdesc='NimaOS Installer Framework'
arch=(any)
depends=('squashfs-tools' 'arch-install-scripts' 'util-linux' 'parted')
provides=('nimaos-inst')
conflicts=('nimaos-inst')
source=('git-inst::git+https://github.com/NimaOS/nimaos-inst.git')
sha256sums=('SKIP')

pkgver() {
    cd "${srcdir}/git-inst"
    printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cd "${srcdir}/git-inst"
    install -Dm755 blend-inst -t "${pkgdir}/usr/bin/"
}

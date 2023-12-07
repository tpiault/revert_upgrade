pkgname=revert_upgrade
pkgver=1.0.0beta
pkgrel=1
pkgdesc="Downgrade all upgraded packages at once easily"
url="https://github.com/tpiault/revert_upgrade"
source=(
    "preupgrade_save"
    "preupgrade_save.hook"
    "revert_upgrade")
arch=("any")
depends=(expac)
sha256sums=('d88fc8f62af72ee750ce9af96e4c81d1cc81d900d9ec0bd0bb3ef68313c11238'
            '367a2773ecfeb24daff368786535ac0d0b84ed5dac29a4b7b72bae660d410f4e'
            'b2bcfcb577774dcd6e5ee703a55f02251ab2f1896a75f9bcb595e1009e342efc')

package() {
    install -D revert_upgrade "${pkgdir}/usr/bin/revert_upgrade"
    install -D preupgrade_save "${pkgdir}/usr/share/libalpm/scripts/preupgrade_save"
    mkdir -p "${pkgdir}/usr/share/libalpm/hooks/"
    cp preupgrade_save.hook "${pkgdir}/usr/share/libalpm/hooks/"
}

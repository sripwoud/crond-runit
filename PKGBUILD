# Maintainer: sripwoud <me@sripwoud.xyz>
_pkgname=crond
pkgname=${_pkgname}-runit
pkgver=1.0
pkgrel=1
pkgdesc="Custom ${_pkgname} runit service"
arch=('any')
url="https://github.com/sripwoud/${_pkgname}-runit"
license=('AGPL-3.0-only')
depends=('runit' 'dcron-git')
source=("run" "run.asc")
validpgpkeys=('D99B40AC0CE81A5FF8B8456F6296216946C1B36A')
sha256sums=('814dea14ac612125e97dcc1d619219b2c9dfc14850bf48d858421fb2c98eca12' 'SKIP')
install=run.install

package() {
    install -Dm755 "${srcdir}/run" "${pkgdir}/etc/runit/sv/${_pkgname}/run"
}

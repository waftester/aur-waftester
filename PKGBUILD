# Maintainer: WAFtester <info@waftester.com>
pkgname=waftester-bin
pkgver=2.9.5
pkgrel=1
pkgdesc="WAF security testing CLI — detect, benchmark, and bypass web application firewalls"
arch=('x86_64' 'aarch64')
url="https://waftester.com"
license=('custom:BSL-1.1')
provides=('waftester')
conflicts=('waftester')

source_x86_64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_x86_64.tar.gz")
source_aarch64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_arm64.tar.gz")
sha256sums_x86_64=('8467ff0bfeebdecfc17624f228e265d4e3bd19379c777e9366ef246a1d581423')
sha256sums_aarch64=('7af69168998bc59e72b7a6fdbb9585e7cd463d1f0410ba4b48f0f990562ae5b8')

package() {
  install -Dm755 waf-tester "${pkgdir}/usr/bin/waf-tester"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
  install -Dm644 README.md "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}

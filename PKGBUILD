# Maintainer: WAFtester <info@waftester.com>
pkgname=waftester-bin
pkgver=2.9.10
pkgrel=1
pkgdesc="WAF security testing CLI — detect, benchmark, and bypass web application firewalls"
arch=('x86_64' 'aarch64')
url="https://waftester.com"
license=('custom:BSL-1.1')
provides=('waftester')
conflicts=('waftester')

source_x86_64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_x86_64.tar.gz")
source_aarch64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_arm64.tar.gz")
sha256sums_x86_64=('88f3dc779397b284bb64574cc05970704acdd367d45178c192b0e82207a30ceb')
sha256sums_aarch64=('e6d13c3f5ce279c8da7cc691608e5bac3d37e10301fcb445aec5c7c8c53e667d')

package() {
  install -Dm755 waf-tester "${pkgdir}/usr/bin/waf-tester"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
  install -Dm644 README.md "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}

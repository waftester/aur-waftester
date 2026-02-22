# Maintainer: WAFtester <info@waftester.com>
pkgname=waftester-bin
pkgver=2.9.25
pkgrel=1
pkgdesc="WAF security testing CLI — detect, benchmark, and bypass web application firewalls"
arch=('x86_64' 'aarch64')
url="https://waftester.com"
license=('custom:BSL-1.1')
provides=('waftester')
conflicts=('waftester')

source_x86_64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_x86_64.tar.gz")
source_aarch64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_arm64.tar.gz")
sha256sums_x86_64=('5061fe300e78aa66a983472ff815e3ca9e5b6ea47945303e6d9337645421b43a')
sha256sums_aarch64=('abc23cde630142fbecb7302bf797dcfa369c7b1b2208c44ae2fec05adbfec01f')

package() {
  install -Dm755 waf-tester "${pkgdir}/usr/bin/waf-tester"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
  install -Dm644 README.md "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}

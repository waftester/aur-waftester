# Maintainer: WAFtester <info@waftester.com>
pkgname=waftester-bin
pkgver=2.9.26
pkgrel=1
pkgdesc="WAF security testing CLI — detect, benchmark, and bypass web application firewalls"
arch=('x86_64' 'aarch64')
url="https://waftester.com"
license=('custom:BSL-1.1')
provides=('waftester')
conflicts=('waftester')

source_x86_64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_x86_64.tar.gz")
source_aarch64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_arm64.tar.gz")
sha256sums_x86_64=('77281b5781a50d5ba87f658d0ce7d4e65a3fef9af181671c260cc2e630bb783d')
sha256sums_aarch64=('02fcbb6805968558c3b1d02e8691eb624e0a62091031e5e10af156f107ab5e75')

package() {
  install -Dm755 waf-tester "${pkgdir}/usr/bin/waf-tester"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
  install -Dm644 README.md "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}

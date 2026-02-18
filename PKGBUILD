# Maintainer: WAFtester <info@waftester.com>
pkgname=waftester-bin
pkgver=2.9.12
pkgrel=1
pkgdesc="WAF security testing CLI — detect, benchmark, and bypass web application firewalls"
arch=('x86_64' 'aarch64')
url="https://waftester.com"
license=('custom:BSL-1.1')
provides=('waftester')
conflicts=('waftester')

source_x86_64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_x86_64.tar.gz")
source_aarch64=("https://github.com/waftester/waftester/releases/download/v${pkgver}/waftester_Linux_arm64.tar.gz")
sha256sums_x86_64=('d20e99e53d2d1567e9936e595fef5608a1f4571cd384d49d31826c467aaea99a')
sha256sums_aarch64=('d9b380e37285560199db6c55041dace62996db052b2f8e4a5210c70162d6eb45')

package() {
  install -Dm755 waf-tester "${pkgdir}/usr/bin/waf-tester"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
  install -Dm644 README.md "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}

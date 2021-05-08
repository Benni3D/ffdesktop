# Maintainer: Benjamin Stürz <benni@stuerz.xyz>
pkgname=ffdesktop
pkgver=1.1
pkgrel=1
pkgdesc="Redirect the desktop on X11 to a virtual webcam"
arch=('x86_64')
url="https://github.com/Benni3D/ffdesktop"
license=('MIT')
depends=('ffmpeg' 'v4l2loopback-dkms')
source=("https://github.com/Benni3D/ffdesktop/archive/v${pkgver}.tar.gz")
md5sums=('SKIP')

package() {
   cd "${srcdir}/${pkgname}-${pkgver}"
   install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
   install -Dm755 ffdesktop.sh "${pkgdir}/usr/bin/ffdesktop"
}


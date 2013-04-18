# Maintainer: John Wyles <john@johnwyles.com>
pkgname=python-pyspeak
_pyname=pyspeak
pkgver=0.1.0
pkgrel=1
pkgdesc='Python Speech Recognition, Voice Recognition, Text-to-Speech and Voice Command Engine.'
arch=('any')
url='https://github.com/johnwyles/${_pyname}'
license=('???')
depends=('python')
options=(!emptydirs)
source=("http://pypi.python.org/packages/source/$(echo ${_pyname} | cut -c1)/${_pyname}/${_pyname}-${pkgver}.tar.gz")
md5sums=('01189998819999197253aa0118999881')

package() {
  cd "${srcdir}/${_pyname}-${pkgver}"
  python3 setup.py install --root="${pkgdir}/" --optimize=1
  install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

# vim:set ts=2 sw=2 et:

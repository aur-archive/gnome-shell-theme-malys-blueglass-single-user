### Author: ~malys777 <http://malys777.deviantart.com/>
# Maintainer  sanderd17 < sanderd17 AT gmail DOT com >

pkgname=gnome-shell-theme-malys-blueglass-single-user
pkgver=0.6
pkgrel=1
pkgdesc="Malys GNOME Shell Theme. No system wide installation."
url="http://malys777.deviantart.com/#/d3oj0sl"
license=('cc-by-nc-sa-3.0')
arch=('any')
depends=('gnome-shell')
makedepends=('unzip')
optdepends=('gnome-shell-extension-user-theme: User Theme extension for GNOME Shell'
            'gnome-tweak-tool: A tool to customize advanced GNOME 3 options.')
source=(http://www.deviantart.com/download/222596805/malys___blueglass_0_6_by_malys777-d3oj0sl.zip)
DLAGENTS=('http::/usr/bin/wget -c -t 3 --waitretry=3 -H -U Mozilla -O %o %u')
md5sums=('d73d4ee296d69fabdd57b517550ec5be')



package() {
  mkdir -p ${pkgdir}$HOME/.themes/Malys-BlueGlass

  unzip -o malys___blueglass_0_6_by_malys777-d3oj0sl.zip
  ls -lrta $srcdir
  cp -R $srcdir/gnome-shell-theme-malys-blueglass/malys-blueglass/gnome-shell $pkgdir$HOME/.themes/Malys-BlueGlass/

  chmod -R 755 ${pkgdir}$HOME/.themes/Malys-BlueGlass
}




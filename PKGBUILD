# Contributor: gareth_c
# Maintainer: Ner0

pkgname=cinnamon-applet-iconized-window-list
pkgver=2.7
pkgrel=1
pkgdesc="A window list with window previews and win7 like favorites."
arch=('any')
url="http://cinnamon-spices.linuxmint.com/applets/view/16"
license=('GPL')
groups=('cinnamon-applets')
depends=('cinnamon')
install=$pkgname.install
source=("http://cinnamon-spices.linuxmint.com/uploads/applets/3IDA-0443-B57M.zip")
md5sums=('74de2786e77a40bb1a47ae4187f4bc39')

package() {
  find WindowListGroup\@jake.phy\@gmail.com/ -type f -not -name *~ -and -not -name install.sh -and -not -name *.xml -exec install -Dm644 '{}' "$pkgdir/usr/share/cinnamon/applets/{}" \;

  install -Dm644 WindowListGroup\@jake.phy@gmail.com/*.xml "$pkgdir/usr/share/glib-2.0/schemas/org.cinnamon.applets.windowListGroup.gschema.xml"

  chmod +x "$pkgdir/usr/share/cinnamon/applets/WindowListGroup@jake.phy@gmail.com"/*.py
}

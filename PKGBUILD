pkgname=rea
pkgver=20120811
pkgrel=1
pkgdesc="bot for irc.freenode.#geekfeminism"
arch=(i686 x86_64)
depends=(python2-coverage python2-mock python2-nose python2-pyopenssl twisted)
makedepends=(git automake autoconf)
url=https://github.com/yardenac/rea
license=GPL
backup=(etc/screenrc etc/pam.d/screen)
#install=screen.install
_gitroot=git://github.com/yardenac/rea.git
_gitname=rea

build() {
	 cd $srcdir
	 [ -d $srcdir/$_gitname ] \
		  && cd $_gitname && git pull origin \
		  || git clone $_gitroot
}
package() {
	 cd $srcdir/$_gitname/src
}

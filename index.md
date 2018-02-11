# Milo's NBPS GPA Calculator

---

## Download and Use

Click [here](https://github.com/Myl0g/gpacalc_cpp/releases/latest) to download the latest version.

### Mac

Move the downloaded file to an uncluttered place so you don't lose it (e.g. your Desktop, Documents, Home folder, etc).

If the file is titled "gpacalc-mac-...", then double-click it to un-zip the actual app.

Double-click the file "gpacalc". You should see a warning saying the app can't be opened since it's from an unidentified developer.
Hit "OK", then right-click "gpacalc" and select "Open". The same prompt should appear, but with an option to open it. Click that option.

### Windows

Un-zip the downloaded file, and try running the file from Windows Explorer.

### Linux

Run the following in the terminal, substituting the "<>":

```
tar xvf <path to downloaded file>
chmod +x ./gpacalc
```

You can now run the calculator normally.

#### Arch Linux

Here's a PKGBUILD for you to use (please **insert the correct version number**):

```
pkgname=gpacalc-bin
pkgver=
pkgrel=1
epoch=
pkgdesc="NBPS GPA Calculator (C++ Edition)"
arch=(x86_64)
url="http://github.com/Myl0g/gpacalc_cpp"
license=('GPL')
depends=('gcc-libs')
source=("https://github.com/Myl0g/gpacalc_cpp/releases/download/v${pkgver}/gpacalc-linux-${pkgver}.tar.xz")

package() {
	install -d "${pkgdir}/usr/bin"
	install "${srcdir}/gpacalc" "${pkgdir}/usr/bin"
}
```

Remember to run `makepkg -g >> PKGBUILD`.

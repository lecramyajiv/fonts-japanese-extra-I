## UmePlus CL fonts

UmePlus CL (CLassical style) fonts are modified Ume fonts for Japanese.

<http://www.geocities.jp/ep3797/modified_fonts_01.html>

I used these fonts for UmePlus CL fonts:

- Kanji, hiragana, katakana = Ume fonts

  <https://osdn.net/projects/ume-font/releases/>

- Alphabet, Full width alphabet = M+ fonts

  <https://osdn.net/projects/mplus-fonts/releases/>

Thanks to the authors.

### License

Ume fonts, M+ fonts: See docs-{ume,mplus}.

fontforge-scripts: Public Domain.

### Author

UTUMI Hirosi (utuhiro78 at yahoo dot co dot jp)

### How to update UmePlus fonts

1. Install fontforge

  ```
  $ sudo pacman -S fontforge
  ```

2. Extract files

  ```
  $ mkdir umeplus-tmp
  $ mv mplus-TESTFLIGHT-063.tar.xz umeplus-tmp/
  $ mv umefont_670.7z umeplus-tmp/
  $ mv umeplus-cl-fonts-20180604.tar.xz umeplus-tmp/
  $ cd umeplus-tmp/
  $ tar xf umeplus-cl-fonts-20180604.tar.xz
  $ mv umeplus-cl-fonts-20180604 umeplus-cl-fonts-dev
  $ mv umeplus-fonts-cl-dev/update-umeplus-cl.sh .
  ```

3. Update "update-umeplus-cl.sh"

  ```
  $ leafpad update-umeplus-cl.sh
  ```

  Change the lines:

  ```
  MPLUSVER="063"
  UMEVER="670"
  UMEPLUSVER="20180604"
  ```

4. Update UmePlus CL fonts

  ```
  $ ./update-umeplus-cl.sh
  ```

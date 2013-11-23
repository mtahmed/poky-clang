# poky

This repository mirrors the official yocto poky repository at
[git://git.yoctoproject.org/poky](git://git.yoctoproject.org/poky)
and contains additional patches to help compile at least the
`core-image-minimal` using clang.

See [meta-tc-llvm](https://github.com/mtahmed/meta-tc-llvm). It's
a secondary toolchain layer which needs to be added to this poky
to help it compile using clang.

## Installation

Simply clone this repository and add the `meta-tc-llvm` layer.

```bash
git clone https://github.com/mtahmed/poky.git
cd poky
git clone https://github.com/mtahmed/meta-tc-llvm.git
```

All the required patches are already in poky. For configuration
specific to `meta-tc-llvm` layer, see the `meta-tc-llvm` link above.

## Patches

These are the set of patches already included in this poky:

- [busybox: find-get-rid-of-nested-functions.patch](https://github.com/mtahmed/poky/blob/master/meta/recipes-core/busybox/busybox-1.21.1/find-get-rid-of-nested-functions.patch)
- [ncurses: fix-types-in-constructor-declaration.patch](https://github.com/mtahmed/poky/blob/master/meta/recipes-core/ncurses/ncurses-5.9/fix-types-in-constructor-declaration.patch)


## Contact

- Muhammad Tauqir Ahmad
- muhammad.tauqir.ahmad@gmail.com
- [csclub.uwaterloo.ca/~mtahmed](http://csclub.uwaterloo.ca/~mtahmed)

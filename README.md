ZenFone boot tools
==================

Fork from https://github.com/sndnvaps/intel-boot-tools

Tools to pack/unpack intel osimage boot images


### Build

- run `make` to build tools: `pack_intel` & `unpack_intel`


### Usage

To build boot.img (or recovery.img) from custom kernel (bzImage) and initrd (ramdisk.cpio.gz), use original boot.img (or recovery.img) as input:

	$ pack_intel boot.img bzImage ramdisk.cpio.gz cmdline new_boot.img

To extract kernel (bzImage) and initrd (ramdisk.cpio.gz) from boot.img (or recovery.img):

	$ unpack_intel boot.img bzImage ramdisk.cpio.gz

# Configs for OpenWrt-1505-Custom repo

This configs are intended for use with OpenWrt-1505-Custom repo, wnr2200ru+custom branch.
USE AT YOUR OWN RISK!

## netgear-wnr2200ru.diffconfig

Config for NETGEAR WNR2200 router (Russian revision). Included stuff that needed for relatively usable LXC support.
Using glibc to improve compatibility with debian-mips binaries, and minimum compression for squashfs to improve performance.
Image built with such configuration only fits in 16MiB router revision. If you trying to build image for router revision with 8MiB flash - switch to uclibc and change CONFIG_TARGET_SQUASHFS_BLOCK_SIZE at least to 64.

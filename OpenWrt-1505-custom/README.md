# Configs for OpenWrt-1505-Custom repo

This configs are intended for use with OpenWrt-1505-Custom repo, "custom" branch.
USE AT YOUR OWN RISK!

## tp-link-wr842nd-v1.diffconfig

Config for TP-Link TL-WR842ND v1 router. Only essential stuff for everyday SOHO-router usage added to image.
Features that included in addition to minimal config: ipv6+tunnel support, udpxy igmp forwarder,
USB-drives with ext4-fs support, virtual ethernet driver + ip utility, iperf3 utility,
pppol2tp support + xl2tpd daemon (extra packages and configuration needed for encryption support).
LXC support is disabled, but glibc is used to provide compatibility with debian-mips binaries. Other components available as external packages.

## kvm.diffconfig

Config for running openwrt with qemu-kvm 32-bit x86 virtualization technology.
This config based on netgear-wnr2200ru.diffconfig, with additions for network-fs and connectivity support.
Included stuff that needed for relatively usable LXC support.
Using glibc by default to improve compatibility with typical x86-32bit-linux' binaries.
Using virtual mtd+squashfs layout: you must manually use "dd" to copy image (with start at sector 0) to virtual drive with bigger size used by qemu-kvm as boot drive,
remaining free space will be automatically formatted as overlay on first boot.


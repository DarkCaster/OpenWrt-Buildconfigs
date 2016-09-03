# Configs for OpenWrt-1505-Custom repo

This configs are intended for use with OpenWrt-1505-Custom repo, "custom" branch.
USE AT YOUR OWN RISK!

## tp-link-wr842nd-v1.diffconfig

Config for TP-Link TL-WR842ND v1 router. Only essential stuff for everyday SOHO-router usage added to image.
Features that included in addition to minimal config: ipv6+tunnel support, udpxy igmp forwarder,
USB-drives with ext4-fs support, virtual ethernet driver + ip utility, iperf3 utility,
pppol2tp support + xl2tpd daemon (extra packages and configuration needed for encryption support).
LXC support is disabled, but glibc is used to provide compatibility with debian-mips binaries. Other components available as external packages.


my-kernel-config
================

Git repository for my laptop kernel config (Comapl IFL90)

Features:
* 1000Hz;
* Core2 optimizations (Intel T7500);
* Lean kernel - got rid of some "bloat" (but not all I think);
* Frequently used modules are compiled inline;
 * Notorious exceptions: PPTP and Radeon;
* Gzip compressed for performance (will switch to lzo in a next revision);

Tested and working:
* 3D (Mobility Radeon HD3650);
* PPTP VPN;
* OpenVPN;
* Audio (Intel Corporation 82801H (ICH8 Family) HD Audio Controller (rev 03));
* Ethernet (Broadcom Corporation NetLink BCM5787M Gigabit Ethernet PCI Express (rev 02));
* Wlan (Intel Corporation PRO/Wireless 4965 AG or AGN [Kedron] Network Connection (rev 61));
* CPU frequency scaling;
* CPU thermal sensors;

What does not work (so far):
* Virtualbox (requires manual module compilation)

Results:
* Over 1 second saved on boot (my laptop boots in 7 seconds from GRUB2 to GDM, down from 8, so that's about a 15% improvement);
* Very responsive desktop. I can identify the kernel I am running (stock Arch kernel or my custom one) just by playing around in gnome-shell;
* A great learning experience on the kernel (at least I can say I have scratched the surface);

#
# Copyright (C) 2013 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=imx23
BOARDNAME:=Freescale i.MX23 series
FEATURES:=ext4 rtc usb gpio
CFLAGS:=-Os -pipe -march=armv5te -mtune=arm926ej-s -fno-caller-saves
MAINTAINER:=Zoltan HERPAI <wigyori@uid0.hu>
LINUX_VERSION:=3.10
KERNELNAME:="zImage dtbs"
#DEPENDS:=+imx-bootlets

define Target/Description
	Support for Freescale i.MX233-based boards
endef

include $(INCLUDE_DIR)/target.mk

DEFAULT_PACKAGES += kmod-wdt-stmp3xxx

$(eval $(call BuildTarget))

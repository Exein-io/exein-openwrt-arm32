#
# Copyright (C) 2019 Exein
#
# This is free software, licensed under the GNU General Public License v3.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=xtensor
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/xtensor-stack/xtensor.git
PKG_SOURCE_VERSION:=d59ab1dafff4ba419a8b735ff3e951b9f89cedb8
PKG_MIRROR_HASH:=73a598a2ba15799ba64a7609f279f09581333dead68fa3100a9f5a656809b3be
PKG_BUILD_DEPENDS:=xtl

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Exein <info@exein.io>

include $(INCLUDE_DIR)/package.mk


define Package/xtensor
	SECTION:=libs
	CATEGORY:=Tensorflow
	SUBMENU:=Libraries
	TITLE:=Multi-dimensional arrays with broadcasting and lazy computing.
	DEPENDS:=+libstdcpp
endef

define Build/Compile
endef

define Package/xtensor/install
endef

define Build/InstallDev
	$(INSTALL_DIR) $(1)/usr/include/xtensor
	$(CP) -a $(PKG_BUILD_DIR)/include/xtensor $(1)/usr/include
endef

$(eval $(call BuildPackage,xtensor))

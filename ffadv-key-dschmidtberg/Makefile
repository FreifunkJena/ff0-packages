#
# Copyright (C) 2006-2012 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

# Package content copyright (C) 
#      2012 Freifunk Rheinland e. V. <http://www.freifunk-rheinland.net/>


include $(TOPDIR)/rules.mk

PKG_NAME:=ffadv-key-dschmidtberg
PKG_VERSION:=20130309
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/ffadv-key-dschmidtberg
  SECTION:=base
  CATEGORY:=Utilities
  SUBMENU:=Freifunk Advanced
  PKGARCH:=all
  DEFAULT:=n
  TITLE:=SSH maintenance key (FFW DSchmidtberg)
  MAINTAINER:=DSchmidtberg <dschmidtberg@freifunk-wuppertal.net>
  URL:=http://freifunk-rheinland.net
  DEPENDS:=+dropbear
endef

define Package/ffadv-key-dschmidtberg/description
  SSH key for maintenance
endef

define Build/Prepare
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffadv-key-dschmidtberg/install
	mkdir -p $(1)/CONTROL
	$(INSTALL_BIN) ./ipkg/ffadv-key-dschmidtberg.postinst $(1)/CONTROL/postinst
	$(INSTALL_BIN) ./ipkg/ffadv-key-dschmidtberg.postrm $(1)/CONTROL/postrm
endef

$(eval $(call BuildPackage,ffadv-key-dschmidtberg))

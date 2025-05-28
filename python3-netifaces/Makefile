include $(TOPDIR)/rules.mk

PKG_NAME:=python3-netifaces
PKG_VERSION:=0.10.9
PKG_RELEASE:=2
PKG_SOURCE:=netifaces-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/source/n/netifaces/
PKG_HASH:=e5b26853c21c7e6c7b5c3a18c0d37d8618a9e6d05fe71f2db19f4b8e6a5617b9  # You may want to recalculate
PKG_BUILD_DIR:=$(BUILD_DIR)/netifaces-$(PKG_VERSION)

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-netifaces
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Portable network interface information
  URL:=https://github.com/al45tair/netifaces
  DEPENDS:=+libc +python3-light
  MAINTAINER:=Josef Schlehofer <pepe.schlehofer@gmail.com>
endef

define Package/python3-netifaces/description
  Portable network interface information.
endef

$(eval $(call Py3Package,python3-netifaces))
$(eval $(call BuildPackage,python3-netifaces))

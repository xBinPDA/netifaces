include $(TOPDIR)/rules.mk

PKG_NAME:=python-netifaces
PKG_VERSION:=0.11.0
PKG_RELEASE:=1
PYPI_NAME:=netifaces
PKG_HASH:=64ac96978c43edc63090629f2d2e3cbf30e327df2eb4434e36a824f89e26ebfa

PKG_SOURCE:=netifaces-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/source/n/netifaces
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PYPI_NAME)-$(PKG_VERSION)

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/../feeds/packages/lang/python/python3-package.mk

define Package/python3-netifaces
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Python netifaces module
  URL:=https://github.com/al45tair/netifaces
  DEPENDS:=+python3
endef

define Package/python3-netifaces/description
  Portable access to network interface information in Python.
endef

$(eval $(call Py3Package,python3-netifaces))
$(eval $(call BuildPackage,python3-netifaces))

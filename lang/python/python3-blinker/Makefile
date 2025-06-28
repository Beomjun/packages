include $(TOPDIR)/rules.mk

PKG_NAME:=python3-blinker
PKG_VERSION:=1.4
PKG_RELEASE:=1

PYPI_NAME:=blinker
PKG_HASH:=471aee25f3992bd325afa3772f1063dbdbbca947a041b8b89466dc00d606f8b6

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-blinker
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Fast Pythonic object-to-object and broadcast signaling
	URL:=https://pythonhosted.org/blinker/
	DEPENDS:=+python3
endef

define Package/python3-blinker/description
  Blinker provides fast, simple object-to-object and broadcast signaling for Python programs.
endef

$(eval $(call Py3Package,python3-blinker))
$(eval $(call BuildPackage,python3-blinker))
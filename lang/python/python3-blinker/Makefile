include $(TOPDIR)/rules.mk

PKG_NAME:=python3-blinker
PKG_VERSION:=1.9.0
PKG_RELEASE:=1

PYPI_NAME:=blinker
PKG_HASH:=b4ce2265a7abece45e7cc896e98dbebe6cead56bcf805a3d23136d145f5445bf

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-blinker
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Fast Pythonic object-to-object and broadcast signaling
	URL:=https://pythonhosted.org/blinker/
	DEPENDS:=+python3-light
endef

define Package/python3-blinker/description
  Blinker provides fast, simple object-to-object and broadcast signaling for Python programs.
endef

$(eval $(call Py3Package,python3-blinker))
$(eval $(call BuildPackage,python3-blinker))

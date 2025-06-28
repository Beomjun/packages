include $(TOPDIR)/rules.mk

PKG_NAME:=python3-zstandard
PKG_VERSION:=0.23.0
PKG_RELEASE:=1

PYPI_NAME:=zstandard
PKG_HASH:=b2d8c62d08e7255f68f7a740bae85b3c9b8e5466baa9cbf7f57f1cde0ac6bc09

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-zstandard
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Zstandard bindings for Python
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-zstandard))
$(eval $(call BuildPackage,python3-zstandard))

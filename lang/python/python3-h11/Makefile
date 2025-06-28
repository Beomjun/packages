include $(TOPDIR)/rules.mk

PKG_NAME:=python3-h11
PKG_VERSION:=0.9.0
PKG_RELEASE:=1

PYPI_NAME:=h11
PKG_HASH:=33d4bca7be0fa039f4e84d50ab00531047e53d6ee8ffbc83501ea602c169cae1

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-h11
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Pure-Python HTTP/1.1 protocol library
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-h11))
$(eval $(call BuildPackage,python3-h11))
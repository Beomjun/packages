include $(TOPDIR)/rules.mk

PKG_NAME:=python3-zstandard
PKG_VERSION:=0.15.2
PKG_RELEASE:=1

PYPI_NAME:=zstandard
PKG_HASH:=52de08355fd5cfb3ef4533891092bb96229d43c2069703d4aff04fdbedf9c92f

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-zstandard
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Zstandard bindings for Python
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-zstandard))
$(eval $(call BuildPackage,python3-zstandard))

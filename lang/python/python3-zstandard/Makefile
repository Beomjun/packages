include $(TOPDIR)/rules.mk

PKG_NAME:=python3-zstandard
PKG_VERSION:=0.24.0
PKG_RELEASE:=1

PYPI_NAME:=zstandard
PKG_HASH:=fe3198b81c00032326342d973e526803f183f97aa9e9a98e3f897ebafe21178f

HOST_BUILD_DEPENDS:=python-cffi/host

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

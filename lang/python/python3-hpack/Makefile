include $(TOPDIR)/rules.mk

PKG_NAME:=python3-hpack
PKG_VERSION:=4.1.0
PKG_RELEASE:=1

PYPI_NAME:=hpack
PKG_HASH:=ec5eca154f7056aa06f196a557655c5b009b382873ac8d1e66e79e87535f1dca

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-hpack
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=HTTP/2 header encoding for Python
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-hpack))
$(eval $(call BuildPackage,python3-hpack))

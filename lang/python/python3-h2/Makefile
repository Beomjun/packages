include $(TOPDIR)/rules.mk

PKG_NAME:=python3-h2
PKG_VERSION:=4.1.0
PKG_RELEASE:=1

PYPI_NAME:=h2
PKG_HASH:=a83aca08fbe7aacb79fec788c9c0bac936343560ed9ec18b82a13a12c28d2abb

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-h2
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=HTTP/2 protocol stack, written in Python
	DEPENDS:=+python3-light +python3-hyperframe +python3-hpack
endef

$(eval $(call Py3Package,python3-h2))
$(eval $(call BuildPackage,python3-h2))

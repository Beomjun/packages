include $(TOPDIR)/rules.mk

PKG_NAME:=python3-hpack
PKG_VERSION:=3.0.0
PKG_RELEASE:=1

PYPI_NAME:=hpack
PKG_HASH:=8eec9c1f4bfae3408a3f30500261f7e6a65912dc138526ea054f9ad98892e9d2

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-hpack
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=HTTP/2 header encoding for Python
	DEPENDS:=+python3
endef

$(eval $(call Py3Package,python3-hpack))
$(eval $(call BuildPackage,python3-hpack))
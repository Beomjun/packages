include $(TOPDIR)/rules.mk

PKG_NAME:=python3-wsproto
PKG_VERSION:=0.11.0
PKG_RELEASE:=1

PYPI_NAME:=wsproto
PKG_HASH:=02f214f6bb43cda62a511e2e8f1d5fa4703ed83d376d18d042bd2bbf2e995824

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-wsproto
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Pure Python WebSocket protocol stack
	DEPENDS:=+python3-light +python3-h11
endef

$(eval $(call Py3Package,python3-wsproto))
$(eval $(call BuildPackage,python3-wsproto))
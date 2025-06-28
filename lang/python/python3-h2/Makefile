include $(TOPDIR)/rules.mk

PKG_NAME:=python3-h2
PKG_VERSION:=4.0.0
PKG_RELEASE:=1

PYPI_NAME:=h2
PKG_HASH:=bb7ac7099dd67a857ed52c815a6192b6b1f5ba6b516237fc24a085341340593d

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-h2
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=HTTP/2 protocol stack, written in Python
	DEPENDS:=+python3-light +python3-hyperframe +python3-hpack
endef

$(eval $(call Py3Package,python3-h2))
$(eval $(call BuildPackage,python3-h2))
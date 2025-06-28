include $(TOPDIR)/rules.mk

PKG_NAME:=python3-wsproto
PKG_VERSION:=1.2.0
PKG_RELEASE:=1

PYPI_NAME:=wsproto
PKG_HASH:=ad565f26ecb92588a3e43bc3d96164de84cd9902482b130d0ddbaa9664a85065

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-wsproto
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Pure Python WebSocket protocol stack
	DEPENDS:=+python3-light +python3-h11
endef

$(eval $(call Py3Package,python3-wsproto))
$(eval $(call BuildPackage,python3-wsproto))

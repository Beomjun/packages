include $(TOPDIR)/rules.mk

PKG_NAME:=python3-hyperframe
PKG_VERSION:=6.0.1
PKG_RELEASE:=1

PYPI_NAME:=hyperframe
PKG_HASH:=ae510046231dc8e9ecb1a6586f63d2347bf4c8905914aa84ba585ae85f28a914

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-hyperframe
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=HTTP/2 framing layer
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-hyperframe))
$(eval $(call BuildPackage,python3-hyperframe))

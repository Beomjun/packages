include $(TOPDIR)/rules.mk

PKG_NAME:=python3-brotli
PKG_VERSION:=1.0.9
PKG_RELEASE:=1

PYPI_NAME:=Brotli
PKG_HASH:=4d1b810aa0ed773f81dceda2cc7b403d01057458730e309856356d4ef4188438
PKG_SOURCE:=$(PYPI_NAME)-$(PKG_VERSION).zip

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-brotli
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Brotli compression format decoder/encoder
	DEPENDS:=+python3-light +libstdcpp
endef

$(eval $(call Py3Package,python3-brotli))
$(eval $(call BuildPackage,python3-brotli))
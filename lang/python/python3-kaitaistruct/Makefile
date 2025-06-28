include $(TOPDIR)/rules.mk

PKG_NAME:=python3-kaitaistruct
PKG_VERSION:=0.10
PKG_RELEASE:=1

PYPI_NAME:=kaitaistruct
PKG_HASH:=a044dee29173d6afbacf27bcac39daf89b654dd418cfa009ab82d9178a9ae52a

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-kaitaistruct
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Python API for Kaitai Struct
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-kaitaistruct))
$(eval $(call BuildPackage,python3-kaitaistruct))

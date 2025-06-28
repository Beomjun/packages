include $(TOPDIR)/rules.mk

PKG_NAME:=python3-kaitaistruct
PKG_VERSION:=0.9
PKG_RELEASE:=1

PYPI_NAME:=kaitaistruct
PKG_HASH:=3d5845817ec8a4d5504379cc11bd570b038850ee49c4580bc0998c8fb1d327ad

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-kaitaistruct
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Python API for Kaitai Struct
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-kaitaistruct))
$(eval $(call BuildPackage,python3-kaitaistruct))
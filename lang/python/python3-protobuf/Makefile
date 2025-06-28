include $(TOPDIR)/rules.mk

PKG_NAME:=python3-protobuf
PKG_VERSION:=3.20.0
PKG_RELEASE:=1

PYPI_NAME:=protobuf
PKG_HASH:=71b2c3d1cd26ed1ec7c8196834143258b2ad7f444efff26fdc366c6f5e752702

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-protobuf
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Google Protocol Buffers for Python
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-protobuf))
$(eval $(call BuildPackage,python3-protobuf))
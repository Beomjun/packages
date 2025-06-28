include $(TOPDIR)/rules.mk

PKG_NAME:=python3-pylsqpack
PKG_VERSION:=0.3.22
PKG_RELEASE:=1

PYPI_NAME:=pylsqpack
PKG_HASH:=b67f711b3c8370d9f40f7f7f536aa6018d8900fa09fa49f72f0c3f13886cecda

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-pylsqpack
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Python bindings for the ls-qpack library (HTTP/3 support)
	URL:=https://github.com/aiortc/pylsqpack
	DEPENDS:=+python3-light
endef

define Build/Prepare
	$(call Build/Prepare/Default)
	sed -i 's/^license = "BSD-3-Clause"/license = {text = "BSD-3-Clause"}/' $(PKG_BUILD_DIR)/pyproject.toml
endef

$(eval $(call Py3Package,python3-pylsqpack))
$(eval $(call BuildPackage,python3-pylsqpack))

include $(TOPDIR)/rules.mk

PKG_NAME:=python3-ruamel-yaml
PKG_VERSION:=0.18.14
PKG_RELEASE:=1

PYPI_NAME:=ruamel.yaml
PKG_HASH:=7227b76aaec364df15936730efbf7d72b30c0b79b1d578bbb8e3dcb2d81f52b7

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ruamel-yaml
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=ruamel.yaml - YAML 1.2 parser/emitter
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-ruamel-yaml))
$(eval $(call BuildPackage,python3-ruamel-yaml))
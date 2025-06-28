include $(TOPDIR)/rules.mk

PKG_NAME:=python3-pyperclip
PKG_VERSION:=1.8.2
PKG_RELEASE:=1

PYPI_NAME:=pyperclip
PKG_HASH:=105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-pyperclip
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Cross-platform clipboard module for Python
	URL:=https://github.com/asweigart/pyperclip
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-pyperclip))
$(eval $(call BuildPackage,python3-pyperclip))

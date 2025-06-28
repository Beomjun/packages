include $(TOPDIR)/rules.mk

PKG_NAME:=python3-urwid
PKG_VERSION:=2.1.2
PKG_RELEASE:=1

PYPI_NAME:=urwid
PKG_HASH:=588bee9c1cb208d0906a9f73c613d2bd32c3ed3702012f51efe318a3f2127eae

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-urwid
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Console UI library for Python
	DEPENDS:=+python3
endef

$(eval $(call Py3Package,python3-urwid))
$(eval $(call BuildPackage,python3-urwid))
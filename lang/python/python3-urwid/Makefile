include $(TOPDIR)/rules.mk

PKG_NAME:=python3-urwid
PKG_VERSION:=2.6.16
PKG_RELEASE:=1

PYPI_NAME:=urwid
PKG_HASH:=93ad239939e44c385e64aa00027878b9e5c486d59e855ec8ab5b1e1adcdb32a2

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-urwid
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Console UI library for Python
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-urwid))
$(eval $(call BuildPackage,python3-urwid))

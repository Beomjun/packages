include $(TOPDIR)/rules.mk

PKG_NAME:=python3-pyperclip
PKG_VERSION:=1.9.0
PKG_RELEASE:=1

PYPI_NAME:=pyperclip
PKG_HASH:=b7de0142ddc81bfc5c7507eea19da920b92252b548b96186caf94a5e2527d310

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

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

include $(TOPDIR)/rules.mk

PKG_NAME:=python3-pydivert
PKG_VERSION:=2.1.0
PKG_RELEASE:=1

PYPI_NAME:=pydivert
PKG_HASH:=f0e150f4ff591b78e35f514e319561dadff7f24a82186a171dd4d465483de5b4

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-pydivert
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Pythonic binding for WinDivert packet capture (Windows only)
	URL:=https://github.com/ffalcinelli/pydivert
	DEPENDS:=+python3-light
endef

$(eval $(call Py3Package,python3-pydivert))
$(eval $(call BuildPackage,python3-pydivert))

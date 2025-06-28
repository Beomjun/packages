include $(TOPDIR)/rules.mk

PKG_NAME:=python3-ldap3
PKG_VERSION:=2.9.1
PKG_RELEASE:=1

PYPI_NAME:=ldap3
PKG_HASH:=f3e7fc4718e3f09dda568b57100095e0ce58633bcabbed8667ce3f8fbaa4229f

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ldap3
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Strictly RFC 4510 conforming LDAP V3 pure Python client
	URL:=https://github.com/cannatag/ldap3
	DEPENDS:=+python3
endef

$(eval $(call Py3Package,python3-ldap3))
$(eval $(call BuildPackage,python3-ldap3))

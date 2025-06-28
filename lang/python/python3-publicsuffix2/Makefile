include $(TOPDIR)/rules.mk

PKG_NAME:=python3-publicsuffix2
PKG_VERSION:=2.20191221
PKG_RELEASE:=1

PYPI_NAME:=publicsuffix2
PKG_HASH:=00f8cc31aa8d0d5592a5ced19cccba7de428ebca985db26ac852d920ddd6fe7b

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-publicsuffix2
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Get a public suffix for a domain name using the Public Suffix List
	URL:=https://github.com/nexB/python-publicsuffix2
	DEPENDS:=+python3-light
endef

define Build/Prepare
	$(call Build/Prepare/Default)
	$(STAGING_DIR_HOSTPKG)/bin/python$(PYTHON3_VERSION) -m pip install requests
endef

$(eval $(call Py3Package,python3-publicsuffix2))
$(eval $(call BuildPackage,python3-publicsuffix2))

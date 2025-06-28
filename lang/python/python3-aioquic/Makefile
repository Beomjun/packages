include $(TOPDIR)/rules.mk

PKG_NAME:=python3-aioquic
PKG_VERSION:=1.2.0
PKG_RELEASE:=1

PYPI_NAME:=aioquic
PKG_HASH:=f91263bb3f71948c5c8915b4d50ee370004f20a416f67fab3dcc90556c7e7199

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-aioquic
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=QUIC and HTTP/3 implementation in Python
	URL:=https://github.com/aiortc/aioquic
	DEPENDS:=+python3-light +python3-cryptography
endef

$(eval $(call Py3Package,python3-aioquic))
$(eval $(call BuildPackage,python3-aioquic))

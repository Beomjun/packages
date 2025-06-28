include $(TOPDIR)/rules.mk

PKG_NAME:=python3-aioquic
PKG_VERSION:=0.9.25
PKG_RELEASE:=1

PYPI_NAME:=aioquic
PKG_HASH:=70795c78905326d855c2ae524072234aae586c789b81292e272d021e9b0430a3

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

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

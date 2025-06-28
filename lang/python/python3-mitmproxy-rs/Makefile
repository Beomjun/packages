include $(TOPDIR)/rules.mk

PKG_NAME:=python3-mitmproxy-rs
PKG_VERSION:=0.8.0
PKG_RELEASE:=1

PYPI_NAME:=mitmproxy_rs
PKG_HASH:=62ee60b0dc8902c5cd7d59345108486d8d5c8744f2bcbec678009e29f30c84dc

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-mitmproxy-rs
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Rust-powered core for mitmproxy
	URL:=https://github.com/mitmproxy/mitmproxy-rs
	DEPENDS:=+python3-light
endef

define Package/python3-mitmproxy-rs/install
	$(INSTALL_DIR) $(1)/usr/lib/python3.11/site-packages
	$(CP) -r $(PKG_INSTALL_DIR)/usr/lib/python3.11/site-packages/* $(1)/usr/lib/python3.11/site-packages/
endef

$(eval $(call Py3Package,python3-mitmproxy-rs))
$(eval $(call BuildPackage,python3-mitmproxy-rs))
include $(TOPDIR)/rules.mk

PKG_NAME:=python3-mitmproxy-rs
PKG_VERSION:=0.10.7
PKG_RELEASE:=1

PYPI_NAME:=mitmproxy_rs
PKG_HASH:=0959a540766403222464472b64122ac8ccbca66b5f019154496b98e62482277f

HOST_BUILD_DEPENDS:=rust/host

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-mitmproxy-rs
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=Rust-powered core for mitmproxy
	URL:=https://github.com/mitmproxy/mitmproxy-rs
	DEPENDS:=+python3-light
endef

define Build/Prepare
	$(call Build/Prepare/Default)
	$(STAGING_DIR_HOSTPKG)/bin/python3 -m pip install maturin
	[ -e $(STAGING_DIR_HOSTPKG)/lib/python$(PYTHON3_VERSION)/site-packages/bin/maturin ] && \
		cp $(STAGING_DIR_HOSTPKG)/lib/python$(PYTHON3_VERSION)/site-packages/bin/maturin $(STAGING_DIR_HOSTPKG)/bin/maturin || true
endef

$(eval $(call Py3Package,python3-mitmproxy-rs))
$(eval $(call BuildPackage,python3-mitmproxy-rs))

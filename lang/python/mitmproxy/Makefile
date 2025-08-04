include $(TOPDIR)/rules.mk

PKG_NAME:=mitmproxy
PKG_VERSION:=11.0.2
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://downloads.mitmproxy.org/$(PKG_VERSION)
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_HASH=0892e5b618b463308375b4d9f31bda7b19102d86132b6371f37d5924280f9ee0

PKG_LICENSE:=MIT
PKG_MAINTAINER:=Beomjun Kang <kals323@gmail.com>
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/mitmproxy
	SECTION:=lang
	CATEGORY:=Languages
	SUBMENU:=Python
	TITLE:=An interactive TLS-capable intercepting HTTP proxy
	URL:=https://mitmproxy.org
	DEPENDS:=+python3-light +python3-urllib +python3-requests +python3-pyopenssl +python3-certifi +python3-click +python3-sortedcontainers +python3-cryptography +python3-brotli +python3-flask +python3-msgpack +python3-protobuf +python3-ruamel-yaml +python3-zstandard +python3-tornado +python3-wsproto +python3-h11 +python3-h2 +python3-hyperframe +python3-kaitaistruct +python3-blinker +python3-urwid +python3-mitmproxy-rs +python3-pyparsing +python3-hpack +python3-attrs +python3-aioquic +python3-service-identity +python3-pylsqpack +python3-pyperclip +python3-asgiref +python3-ldap3 +python3-passlib +python3-typing-extensions +python3-pydivert +python3-publicsuffix2 +python3-wcwidth +kmod-ipt-socket +kmod-ipt-tproxy
endef

define Package/mitmproxy/description
	mitmproxy is a free and open source interactive HTTPS proxy.
endef

$(eval $(call Py3Package,mitmproxy))
$(eval $(call BuildPackage,mitmproxy))

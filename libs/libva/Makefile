include $(TOPDIR)/rules.mk

PKG_NAME:=libva
PKG_VERSION:=2.21.0
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.xz

PKG_SOURCE_URL:=https://github.com/intel/libva
PKG_SOURCE_PROTO:=git
PKG_SOURCE_VERSION:=0b01aed44ef1a6ad660261284ff266fa812829ef
PKG_SOURCE_DATE:=2024-03-12

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=COPYING
PKG_BUILD_PARALLEL:=1

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/meson.mk

MESON_ARGS += \
	-Ddisable_drm=false \
	-Dwith_x11=no \
	-Dwith_glx=no \
	-Dwith_wayland=no

define Package/libva
  SECTION:=libs
  CATEGORY:=Libraries
  TITLE:=VA-API core library (for FFmpeg 8.0 VAAPI)
  URL:=https://github.com/intel/libva
  DEPENDS:=+libpthread
endef

define Package/libva/description
libva provides the core Video Acceleration API used by FFmpeg (VAAPI).
This package ships the core library and headers/pkg-config for building.
endef

define Package/libva-drm
  SECTION:=libs
  CATEGORY:=Libraries
  TITLE:=VA-API DRM backend
  URL:=https://github.com/intel/libva
  DEPENDS:=+libva +libdrm
endef

define Package/libva-drm/description
DRM backend for libva (vaGetDisplayDRM). Required for VAAPI on Linux without X/Wayland.
endef

define Build/InstallDev
	$(INSTALL_DIR) $(1)/usr/include/va
	$(CP) $(PKG_INSTALL_DIR)/usr/include/va/*.h $(1)/usr/include/va/

	$(INSTALL_DIR) $(1)/usr/lib
	$(CP) $(PKG_INSTALL_DIR)/usr/lib/libva*.so $(1)/usr/lib/

	$(INSTALL_DIR) $(1)/usr/lib/pkgconfig
	$(CP) $(PKG_INSTALL_DIR)/usr/lib/pkgconfig/libva*.pc $(1)/usr/lib/pkgconfig/
endef

define Package/libva/install
	$(INSTALL_DIR) $(1)/usr/lib
	$(CP) $(PKG_INSTALL_DIR)/usr/lib/libva.so.* $(1)/usr/lib/
endef

define Package/libva-drm/install
	$(INSTALL_DIR) $(1)/usr/lib
	$(CP) $(PKG_INSTALL_DIR)/usr/lib/libva-drm.so.* $(1)/usr/lib/
endef

$(eval $(call BuildPackage,libva))
$(eval $(call BuildPackage,libva-drm))

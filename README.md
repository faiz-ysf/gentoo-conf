
# Installing File Manager


For Gentoo with Wayland/Hyprland, here are some excellent file manager options:

## Top Recommendations

**Thunar** (XFCE's file manager)
- Lightweight, fast, and well-maintained
- Excellent Wayland support
- Good plugin ecosystem

Dependencies to emerge:
```bash
sudo emerge -av xfce-base/thunar
sudo emerge -av xfce-extra/thunar-volman  # volume management
sudo emerge -av xfce-extra/thunar-archive-plugin  # archive support
sudo emerge -av xfce-extra/thunar-media-tags-plugin  # media file tags
```

**PCManFM-Qt** (LXQt's file manager)
- Very lightweight and fast
- Native Qt application with good Wayland support
- Clean, simple interface

Dependencies:
```bash
sudo emerge -av x11-misc/pcmanfm-qt
sudo emerge -av sys-auth/polkit-qt  # for admin operations
```

**Dolphin** (KDE's file manager)
- Feature-rich with excellent functionality
- Outstanding Wayland support
- Many advanced features (split view, tabs, etc.)

Dependencies:
```bash
sudo emerge -av kde-apps/dolphin
sudo emerge -av kde-frameworks/kio-extras  # additional protocols
sudo emerge -av kde-apps/ffmpegthumbs  # video thumbnails
```

## Lighter Alternatives

**Nemo** (Cinnamon's file manager)
```bash
sudo emerge -av gnome-extra/nemo
```

**Nautilus** (GNOME's file manager)
```bash
sudo emerge -av gnome-base/nautilus
```

For Hyprland specifically, I'd recommend **Thunar** or **PCManFM-Qt** as they're lightweight and won't pull in heavy desktop environment dependencies. Thunar strikes a nice balance between features and resource usage.

Make sure you have the `wayland` USE flag enabled globally in your `/etc/portage/make.conf` for optimal Wayland support across all applications.
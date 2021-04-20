# QogirBudgie

[![gtk-theme-qogirbudgie](https://snapcraft.io/gtk-theme-qogirbudgie/badge.svg)](https://snapcraft.io/gtk-theme-qogirbudgie)
[![gtk-theme-qogirbudgie](https://snapcraft.io/gtk-theme-qogirbudgie/trending.svg?name=0)](https://snapcraft.io/gtk-theme-qogirbudgie)

[QogirBudgie](https://github.com/ubuntubudgie/qogir-budgie) is the default GTK theme for Ubuntu Budgie 20.04 and newer.

## Install

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/gtk-theme-qogirbudgie)

```
snap install gtk-theme-qogirbudgie
```

To connect the theme to a snapped application, you can run:

```
sudo snap connect [other snap]:gtk-3-themes gtk-theme-qogirbudgie:gtk-3-themes
sudo snap connect [other snap]:gtk-2-themes gtk-theme-qogirbudgie:gtk-2-themes
```

Or, you can connect the QogirBudgie snapped theme to all snapped apps that support theme plugs:

```
for PLUG in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect ${PLUG} gtk-theme-qogirbudgie:gtk-3-themes; done
for PLUG in $(snap connections | grep gtk-common-themes:gtk-2-themes | awk '{print $2}'); do sudo snap connect ${PLUG} gtk-theme-qogirbudgie:gtk-2-themes; done
```

An official snap built with ❤︎ by the Ubuntu Budgie team using configuration at
<https://github.com/ubuntubudgie/gtk-theme-qogirbudgie-snap> and the Qogir theme from the upstream project source <https://github.com/vinceliuice/qogir-budgie>.

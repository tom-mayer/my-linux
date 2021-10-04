# Linux Config

## Fan Control

- thinkfan package

- /etc/thinkfan.conf

- /etc/modprobe.d/thinkfan.conf

  ```
  options thinkpad_acpi fan_control=1
  ```

- /etc/default/thinkfan

  ```
  START=yes
  DAEMON_ARGS="-q"
  ```

## CPU Throttiling

- cpufrequtils package 

  ```
  cpufreq-set -c 0 -u 3.5GHz
  ...
  ```

- make script for up and down throttling, write simple panel plugin and put down into autostart

## XFCE Config

### Globalmenu

- xfce4-topmenu-plugin package
- libtopmenu-gtk3 libtopmenu-qt topmenu-mozilla-extension
- $HOME/.config/gtk-3.0/settings.ini
- $HOME/.gtk2rc

### Compositor

- Disable xfce compositor

- compton autostart

  ```
  compton --backend glx --paint-on-overlay --vsync opengl-swc
  ```

- ~/.compton.conf

### Extra Plugins

- xfce-windowcs-plugin
  - Disable titlebar on maximised windows in xfce settings
- sensors-plugin
  - set permissions for sensors plugin to read sensors,... will be displayed on launch
- cpufreq
- indicator (arch?)
- whisker menu

## Additional Packages

- Docky
- Oh my ZSH (afowler)
- Typora
- TexLive
- IntelliJ
- BTSync
- Thunderbird
- Firefox
  - TreeStyle Tab
  - Colorful Tab
  - Default Zoom Level
- mpv
- deja-dup (Backups)
- Spotify
- Transmission

## Themes / Styles / Fonts

### Fonts

/usr/share/fonts or $HOME/.fonts

- Menlo: Code
- Monaco: Terminal
- Helvetica Neue / San Francisco: System

### Icons

### http://www.ravefinity.com/p/vibrancy-colors-gtk-icon-theme.html

/usr/share/icons

- Vibrancy Full Dark X

### Theme

http://www.ravefinity.com/p/download-ambiance-blackout-flat-colors.html
andreisergiu98/arc-flatabulous-theme

flatabulous-dark / vibrancy colors

/usr/share/themes

- Ambiance Blackout Flat Dark X




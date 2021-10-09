<h1>Feren OS Rounded Corners (fork of hello's KWin-Effect)</h1>

All credits go to the creator of this effect, as well as https://github.com/khanhas/ShapeCorners for code that was added to this fork.

## Installation

### Build Dependencies

To build the packages you have to install some build-tools for your system first. If you already built something from source chances are you might have some of those installed.

#### Ubuntu
```
sudo apt install git cmake g++ gettext extra-cmake-modules qttools5-dev libqt5x11extras5-dev libkf5configwidgets-dev libkf5crash-dev libkf5globalaccel-dev libkf5kio-dev libkf5notifications-dev kinit-dev kwin-dev 
```

#### Arch Linux
```
sudo pacman -S cmake extra-cmake-modules kdecoration qt5-declarative qt5-x11extras
```

#### Fedora
```
sudo dnf install cmake extra-cmake-modules "cmake(Qt5Core)" "cmake(Qt5Gui)" "cmake(Qt5DBus)" "cmake(Qt5X11Extras)" "cmake(KF5GuiAddons)" "cmake(KF5WindowSystem)" "cmake(KF5I18n)" "cmake(KDecoration2)" "cmake(KF5CoreAddons)" "cmake(KF5ConfigWidgets)" "cmake(Qt5UiTools)" "cmake(KF5GlobalAccel)" kwin-devel libepoxy-devel "cmake(KF5Init)" "cmake(KF5Crash)" "cmake(KF5KIO)" "cmake(KF5Notifications)" kf5-kpackage-devel
```

#### openSUSE
```
sudo zypper install cmake gcc-c++ extra-cmake-modules libQt5Gui-devel libQt5DBus-devel libqt5-qttools-devel libqt5-qtx11extras-devel libQt5OpenGL-devel libQt5Network-devel libepoxy-devel kconfig-devel kconfigwidgets-devel kcrash-devel kglobalaccel-devel ki18n-devel kio-devel kservice-devel kinit-devel knotifications-devel kwindowsystem-devel kguiaddons-devel kpackage-devel kwin5-devel xcb-util-devel xcb-util-cursor-devel xcb-util-wm-devel xcb-util-keysyms-devel
```

If your system is not listed above or there are packages missing in this list, please open an issue or pull request so it can be fixed.

### Manual Installation
Clone the repository and create the build directory:
```
git clone https://github.com/feren-OS/hello-Rounded-Corners
cd hello-Rounded-Corners && cd kwin-effects && mkdir build && cd build
```

Start building with cmake:
```
cmake -DCMAKE_INSTALL_PREFIX=/usr ..
make
sudo make install
```

Finally restart KWin to clear their cache:
```
kwin_x11 --replace &
```

You should now be able to use KDE's system settings to enable the rounding.

## Donate

<b>This below portion has been kept in from the origin of this code, out of due respect.</b>

People have asked me to donate because they enjoyed these tools. Here's how you can donate:

1) Open your favorite search engine
2) Type in "donate homeless in my area" or "donate kids in my area" or similar, you get the idea
3) Donate whatever you would've given to me, to those organizations instead

### Why can't I donate to you?

It's not that I don't want or need the money, but I'm blessed enough to have a roof over my head, food to eat, am generally healthy and have access to machines that allow me to create. Your money can help people in need or projects that help people.

If you live in Germany, here are some projects I personally have donated to and am a believer of:

### Children's Hospice Sternenbrücke

Providing help to families whose children are terminally ill, giving them a nice place to be in for the last moments of their short lives, easing the burden of the parents and even helping families after their child's untimely demise.

https://sternenbruecke.de/jetzt-spenden/paypal

### Streetmagazine Hinz&Kunzt

Project to give homeless people a chance to reclaim their lives and get back on track. Similar to "Big Issue", but on a regional level.

https://www.hinzundkunzt.de/helfen/online-spenden/

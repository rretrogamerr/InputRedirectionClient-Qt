# InputRedirectionClient-Qt
Input redirection client for the 3DS using QtGamepad

Supported platforms:

* Windows (via xinput, if you don't have a Xbox controller you should use x360ce)
* Linux (via evdev)
* OSX
* maybe others?

If you have multiple controllers connected at the same time, this software will combine their inputs.

## Build (Fedora 43)

Dependencies:

```
sudo dnf install gcc-c++ make qt5-qtbase-devel qt5-qtgamepad-devel
```

Build:

```
mkdir -p build
cd build
qmake-qt5 ../InputRedirectionClient-Qt.pro
make -j"$(nproc)"
```
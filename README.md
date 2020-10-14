# A time management utility for GNOME

GNOME Pomodoro is a small application that helps managing time according to [Pomodoro Technique](http://en.wikipedia.org/wiki/Pomodoro_technique). It intends to improve productivity and focus by taking short breaks. It
uses [GNOME](http://www.gnome.org/gnome-3/) technologies, and so it has complete integration with the GNOME desktop environment. For more general information about Pomodoro please visit our website at

https://gnomepomodoro.org

## How to compile

Make sure you have all the requiered dependencies first:

``` sh
sudo apt-get install gettext valac pkg-config desktop-file-utils appstream-util libglib2.0-dev gsettings-desktop-schemas-dev gobject-introspection libgirepository1.0-dev libgstreamer1.0-dev libgtk-3-dev libcanberra-dev libpeas-dev autoconf-archive libgom-1.0-dev libappstream-glib-dev
```

Clone the branch that matches your gnome shell version. For 3.36, you would do:

``` sh
git clone -b gnome-3.36 https://github.com/codito/gnome-pomodoro.git
```

Then, inside the repo directory, run:

``` sh
./autogen.sh --prefix=/usr --datadir=/usr/share
make
sudo make install
```

This software is licensed under the [GPL](https://raw.github.com/codito/gnome-shell-pomodoro/master/COPYING).

*This project is not affiliated with, authorized by, sponsored by, or otherwise approved by GNOME Foundation and/or the Pomodoro Technique®. The GNOME logo and GNOME name are registered trademarks or trademarks of GNOME Foundation in the United States or other countries. The Pomodoro Technique® and Pomodoro™ are registered trademarks of Francesco Cirillo.*

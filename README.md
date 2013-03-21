openlase-mame
=============

A very crude first attempt at interfacing MAME vector games to openlase for laser projector display.  The performance is acceptable for Asteroids, the rest of the vector games are currently to intense without further optimizations.

To build on Ubuntu that still has xmame <= 10.04

    sudo apt-get build-dep xmame
    cd xmame-0.106
    make

To run:

    copy or link xmamerc into $HOME/.xmame directory
    update rompath in $HOME/.xmame/xmamerc to point to where your roms are
    start up openlase (ie jackctl, etc)
    cd xmame-0.106
    ./xmame.x11 asteroid


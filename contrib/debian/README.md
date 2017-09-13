
Debian
====================
This directory contains files used to package bitcoind/bitcoin-qt
for Debian-based Linux systems. If you compile bitcoind/bitcoin-qt yourself, there are some useful files here.

To add URI support and clickable links (arepacoin:<Arepacoin addres>) for the Arepacoin Core QT wallet

This can be installed for either all users or the current user

### All users

#### Install desktop shortcut
    cd arepacoin
    sudo desktop-file-validate ./contrib/debian/arepacoin-qt.desktop # See Note
    sudo cp ./contrib/debian/arepacoin-qt.desktop /usr/share/applications/
    sudo update-desktop-database

#### Install icon graphics
    sudo cp share/pixmaps/arepacoin128.png /usr/share/pixmaps/

### Current user

#### Install desktop shortcut
    cd arepacoin
    sudo desktop-file-validate ./contrib/debian/arepacoin-qt.desktop # Check paths in arepacoin-qt.desktop match the installation path usually /usr/local/bin
    sudo cp ./contrib/debian/arepacoin-qt.desktop ~/.local/share/applications/
    sudo update-desktop-database

#### Install icon graphics
    sudo cp share/pixmaps/arepacoin128.png /usr/share/pixmaps/


**Note:** If you build yourself, you will either need to modify the paths in
the .desktop file or copy arepacoin-qt or symlink your arepacoin-qt binary to `/usr/local/bin`
and copy the `../../share/pixmaps/arepacoin128.png` to `/usr/share/pixmaps`


KDE
====================
bitcoin-qt.protocol (KDE)
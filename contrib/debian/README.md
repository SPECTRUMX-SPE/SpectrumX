
Debian
====================
This directory contains files used to package spectrumxd/spectrumx-qt
for Debian-based Linux systems. If you compile spectrumxd/spectrumx-qt yourself, there are some useful files here.

## spectrumx: URI support ##


spectrumx-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install spectrumx-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your spectrumxqt binary to `/usr/bin`
and the `../../share/pixmaps/spectrumx128.png` to `/usr/share/pixmaps`

spectrumx-qt.protocol (KDE)


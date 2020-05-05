
Debian
====================
This directory contains files used to package sprintd/sprint-qt
for Debian-based Linux systems. If you compile sprintd/sprint-qt yourself, there are some useful files here.

## sprint: URI support ##


sprint-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install sprint-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your sprint-qt binary to `/usr/bin`
and the `../../share/pixmaps/sprint128.png` to `/usr/share/pixmaps`

sprint-qt.protocol (KDE)


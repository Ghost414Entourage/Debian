# Debian

https://novnc.com/noVNC/docs/EMBEDDING.html

sudo apt-get install gnome-core gnome-panel task-gnome-desktop tightvncserver

sudo tightvncserver


tightvncserver -kill :1


mkdir .vnc

cd .vnc

nano xstartup 

#!/bin/sh
unset SESSION_MANAGER
unset DBUS_SESSION_BUS_ADDRESS

xsetroot -solid grey
x-terminal-emulator -geometry 80x24+10+10 -ls -title "$VNCDESKTOP Desktop" &

# Fix GNOME keyboard issue
export XKL_XMODMAP_DISABLE=1

# Launch GNOME components
gnome-panel &
nautilus &
gnome-settings-daemon &
gnome-session &






vncserver

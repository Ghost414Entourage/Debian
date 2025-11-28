# Debian

https://novnc.com/noVNC/docs/EMBEDDING.html

sudo apt-get install gnome-core gnome-panel task-gnome-desktop tightvncserver

sudo tightvncserver

mkdir .vnc

cd .vnc

nano xstartup 

xsetroot -solid grey
x-terminal-emulator -geometry 80x24+10+10 -ls -title "$VNCDESKTOP Desktop" &
#x-window-manager &

# Fix to make GNOME work
export XKL_XMODMAP_DISABLE=1
/etc/X11/Xsession

#gnome-session &
gnome-panel &
nautilus &





vncserver

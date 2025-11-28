# Debian

apt install snapd

snap install core

export PATH=$PATH:/snap/bin

echo 'export PATH=$PATH:/snap/bin' > /etc/profile.d/snap_path.sh

source /etc/profile.d/snap_path.sh

echo $PATH

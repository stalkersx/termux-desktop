RUNNING LINUX ON TERMUX

info :
  |__ Install distro terlebuh dahulu lalu install desktop nya, pilih 1 metode penginstalan distro

INSTALL WITH SCRIPTS DISTRO FILE :
- ! pilih 1 distro yang tersedia
- ! copy file distro ke folder tempat menyimpan berkas linux nantinya
- $ cp nama_distro.sh /path/directory
- $ cd /path/directory/nama_distro.sh
- $ chmod +x nama_distro.sh
- $ ./nama_distro.sh

INSTALL WITH PROOT-DISTRO :
- $ apt install proot proot-distro pulseaudio
- $ proot-distro list
- $ proot-distro install nama_distro
- $ echo "pulseaudio --start --load=\"module-native-protocol-tcp auth-ip-acl=127.0.0.1 auth-anonymous=1\" --exit-idle-time=-1" >> $PREFIX/etc/profile
- $ proot-distro login nama_distro
- $ proot-distro login nama_distro --user nama_user

INSTALL DESKTOP LINUX :
- ! pindahkan folder < install-dekstop > ke home terminal distro yang terinstall
- $ cd install-desktop
- $ chmod +x desktop-linux
- $ cp desktop-linux /usr/bin
- $ desktop-linux
- $ desktop-linux <ukuran layar hp>
- ! mulai otomatis
- $ echo "desktop-linux" >> /etc/profile
- ! hapus mulai otomatis edit /etc/profile dan hapus command < desktop-linux >
- ! install aplikasi bvnc.apk di playstore
- ! input host : 127.0.0.1 dan password vnc

by : @stalkersx

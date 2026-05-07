# thin-client
 
1. update sistem dan install ltsp

sudo add-apt-repository ppa:ltsp/ppa -y
sudo apt update

apt install --install-recommends ltsp ltsp-binaries dnsmasq nfs-kernel-server openssh-server squashfs-tools ethtool net-tools epoptes
gpasswd -a administrator epoptes

2. konfigurasi network

ltsp dnsmasq

3. buat image

ltsp image /

4. konfigurasi ipxe

ltsp ipxe

5. tambahkan .0 di ipxe dan kpxe agar bios dapat membacanya
6. konfigurasi nfs

ltsp nfs

7. generate img

ltsp initrd

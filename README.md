# VirtualBox_OSE_Setup

Setting up VBox bridge network and static IPs:

[root@localhost network-scripts]# history
    1  cd /etc/sysconfig/network-scripts/
    2  cp ifcfg-enp0s3 ifcfg-enp0s3.bak
    3  vi ifcfg-enp0s3
    4  systemctl stop NetworkManager.service
    5  systemctl disable NetworkManager.service
    6  vi ifcfg-enp0s3
    7  vi /etc/resolv.conf 
    8  systemctl restart network
    9  systemctl network status
   10  systemctl status network
   11  ifconfig
   12  ip addr show
   13  vi ifcfg-enp0s3
   14  ping google.com
   15  vi /etc/hostname
   16  ls -al
   17  scp ifcfg-enp0s3 root@192.168.1.103:/etc/sysconfig/network-scripts/ifcfg-enp0s3.bak
   18  vi ifcfg-enp0s3
   19  systemctl restart network
   20  systemctl status network
   21  ifconfig
   22  ip addr show

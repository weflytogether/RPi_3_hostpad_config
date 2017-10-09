# RPi_3_hostpad_config

1) install Raspbian stretch lite to sd card (https://www.raspberrypi.org/downloads/raspbian/)

2) create a empty file called "ssh" in the boot partition in sd card to enable ssh access

3) boot sd card system, log in using pi/raspberry, and install needed packeges

4) setup WiFi hotspot based on https://frillip.com/using-your-raspberry-pi-3-as-a-wifi-access-point-with-hostapd/
   |in /etc/network/interfaces, 
     a) the commented line must be deleted, 
     b) eth0 config need to be added "auto eth0; iface eth0 inet dhcp"
   |for dnsmasq, the dhcp lease file is /var/lib/misc/dnsmasq.leases

5) all config files are organized as them in etc folder

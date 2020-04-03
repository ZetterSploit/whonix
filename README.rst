# whonix for virtualbox installation protocol

# download whonix
  go to https://www.whonix.org/wiki/VirtualBox
  select Whonix with CLI.
  select download
  
# install whonix  
  add whonix to virtualbox, double click on the .ova file
  
  remove Whonix-Workstation, in virtualbox delete whonix-workatation
  
  start Whonix-Gateway
  caution : "us" keyboard
  login : user
  password : changeme

  sudo apt update
  sudo apt full-ugrade
  reboot
  whonixcheck
  
  whonix dashboard
  type : nyx
  whonix new identity
  type : n
  whonix menu
  type : m
  
  connect to the whonix gateway from another unix system
  nano /etc/network/interfaces
# add or adjuste
auto eth0
iface eth0 inet static
address 10.152.152.11
netmask 255.255.192.0
gateway 10.152.152.10

nano /etc/resolv.conf
nameserver 10.152.152.10

reboot

configure virtualbox gateway
select interne network and after whonix

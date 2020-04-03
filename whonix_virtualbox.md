# whonix for virtualbox

[+] download whonix

  go to https://www.whonix.org/wiki/VirtualBox
  select Whonix with CLI.
  select download
  
[+] install whonix  

  add whonix to virtualbox, double click on the .ova file
  remove Whonix-Workstation, in virtualbox delete whonix-workatation
  
[+] start Whonix-Gateway

  caution : "us" keyboard
  
  login : user
  password : changeme

[+] ugrade whonix 
  
  sudo apt update
  sudo apt full-ugrade
  reboot
  
[+] use whonix 

  [+] check system and configuration integrity
    
    whonixchek

  [+] open dashboard
    
    nyx
    
    [+] new identity in dashboard 
    
     n
  
    [+] menu in dashboard
  
     m
  
[+] connect your unix system to whonix gateway
  
  [+] add or adjuste your parametre in /etc/network/interfaces
  
   nano /etc/network/interfaces
  
   auto eth0
   iface eth0 inet static
   address 10.152.152.11
   netmask 255.255.192.0
   gateway 10.152.152.10

  [+] add in /etc/resolv.conf

  nano /etc/resolv.conf
  
  nameserver 10.152.152.10

  reboot

[+] configure virtualbox parametre

  configure virtualbox gateway in configuration > network
  network interface mode : select "internal network"
  name : select "Whonix"

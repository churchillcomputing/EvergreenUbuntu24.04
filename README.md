# EvergreenUbuntu24.04
Evergreen ILS installed on Ubuntu Server 24.04 LTS

Visit churchillcomputing.com for all your library cybersecurity needs.


Download Virtualbox: https://tinyurl.com/n2xwds44 

Ubuntu server login: evergreen
password: evergreen

Run these commands in Ubuntu Server to start Evergreen OPAC & staff client:

su opensrf
password:opensrf

[as opensrf user]

cd /openils/bin

osrf_control --start_all -localhost

exit

[as sudo user]

sudo systemctl restart apache2

sudo systemctl restart websocketd-osrf

Then open your browser and visit <VM_PRIVATE_IP>/eg/opac 
& 
<VM_PRIVATE_IP>/eg/staff

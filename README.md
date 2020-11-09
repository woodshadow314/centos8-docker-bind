# centos8-docker-bind 

mkdir /opt/src
cd /opt/src
git clone https://github.com/woodshadow314/centos8-docker-bind.git
cd centos8-docker-bind/
bash ./bind-install.bash


Install BIND server:...........................................  chcon: cannot access '/etc/rndc.*': No such file or directory
 SUCCESS

Create base BIND configuration:................................   SUCCESS

Restarting BIND:...............................................   SUCCESS


rndc stop
nmtui  # delete DNS 8.8.8.8 and searchdomain

tail -f /var/named/chroot/var/log/*



# install webserver
->lighttpd
https://www.lighttpd.net/download/
move config file to /etc/lighttpd/lighttpd.conf

# compile 
    gcc -o count count.c -lpigpio -lpthread



# add to startup
edit /etc/rc.local and add:
    sudo /home/pi/counter/count 14 -r10 -s10 &



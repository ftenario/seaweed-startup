# seaweed-startup

# Description
This is a startup script for SeadweedFS on Debian Linux. 

# Installation
Copy the file to /etc/init.d and create a symlink on your runlevel.
Ex. "ln -s /etc/init.d/seaweed /etc/rc3.d/S90seaweed"


# Configuration

**BINARY=/usr/local/bin/weed** //Location of your weed binary

**LOG=/techops/weedfs-log/** //Log directory

**TYPE=volume** //Type of weed server. Set this to "volume"

**DIR=/techops/weedfs/** //Location of data

**IP=$(hostname)** //From /etc/hostname. Change this to IP address to be able to link from the master server

**PORT=8080** //Listening port for volume servers

**MSERVER=localhost:9333** //Master server address

**MAX=100** //Maximum number of volumes

# simpleproxmoxgateway
A simple proxmox container that can be used as a gateway for local traffic to the big wide web

That age old problem, you've built an SDN or have a virtual switch, and the local network IP's (in our case 10.0.10.0/24 range) can't see the internet.

IN our demo solution we have a simple Debian Trixie container with eth1 being our public ip/gateway and eth0 being our local network

create run the setup script ont he container - make sure you have all the dependencies installed if it complains do it manually,

set up a crontab

crontab -e

@reboot /root/install

chmod +x the install script

and you're good to go.

Enjoy!

Paul Clevett
Wolf Software Systems Ltd
https://wolf.uk.com

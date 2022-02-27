This is a simple ARP spoofing tool written in Python3
Here we try to poison the ARP table for our router
NOTE: Works in local network

USAGE:
 python3 MalaciousARP.py <router ip> <target ip>
 
Here we take router ip and target ip 
we then get the mac address of both 
then we continously send a malicious packet to both the router and the machine 
we send a packet to router stating we r "target"
and target machine that we are "router"
so now the traffic of the target is passing through our machine and we can sniff the traffic using advanced tools or using my pswdSniffer :)

****IMPORTANT : in our linux machine run this cmd before the script , this would allow the traffic to pass through our machine and not block it, otherwise its a DOS****
 sudo echo 1 >> /proc/sys/net/ipv4/ip_forward

# Block Public DNS

Various devices such as Roku, Chromecast and PS3/PS4 use public DNS servers in preference to the DNS servers configured on the device (or your router). Sometimes the entire device uses the public DNS servers (e.g. Chromecast) and sometimes it's only the individual apps (e.g. Netflix and Dishworld on PS3 or Roku).

Also Netflix App on all devices are using public DNS + it's own DNS.

This breaks SmartDNS services like Wannaflix since other DNS servers end up serving the DNS requests instead of ours. In order to fix this, you will need to take steps to block access to these 3rd party DNS servers on your router. If these devices can't use the public DNS servers, they fallback to using the DNS servers configured on your device or router (e.g. our DNS servers).

### Unsupported Routers

Some routers supplied by ISPs have the advanced settings removed that are required to make these changes. This is a list of known devices:

* Optus Netgear Wireless Cable Voice Gateway CG3000
* Telstra Netgear Wireless Cable Gateway CG3100
* Optus Cisco DPQ 3925-X
* Telstra Cisco EPC 3925

Some other routers simply do no have the option to configure static routes. Here is a list of known devices:

* Apple AirPort Devices
* Most Belkin Routers
* Some Thompson Models

### Generic Instructions

Look for a section on your router to add static routes, there should be room for a network address, subnet mask and gateway. You need to setup the static routes like this:

Network Address: 8.8.8.8\
Subnet Mask: 255.255.255.255\
Gateway: (use the IP address of your router - this is the IP that's in the browser URL)

Network Address: 8.8.4.4\
Subnet Mask: 255.255.255.255\
Gateway: (use the IP address of your router)

**For NETFLIX you also need to add following static routes:**

IP: 108.175.32.0\
Subnet: 255.255.240.0 (or /20)\
Gateway: (use the IP address of your router)

IP: 198.45.48.0\
Subnet: 255.255.240.0 (or /20)\
Gateway: (use the IP address of your router)

IP: 185.2.220.0\
Subnet: 255.255.252.0 (or /22)\
Gateway: (use the IP address of your router)

IP: 37.77.184.0\
Subnet: 255.255.248.0 (or /21)\
Gateway: (use the IP address of your router)

IP: 45.57.0.0\
Subnet: 255.255.128.0 (or /17)\
Gateway: (use the IP address of your router)

**Notes:**

* The "gateway" should be the internal IP address of your router, it will usually start with "192.168." or "10." - make sure you use the internal address, not the public or external address.
* If there is room for a "metric", use the number 2.
* If there is room for an "interface", select either "LAN" or "BRIDGE".

What this does is force your router to route requests to public DNS servers to itself, which will never get routed, so they will never work, and your device will fall back to using the DNS servers you have configured.

**Additional Routes**\
\
Some of our users also suggested the use following static routes. But these may also cause issues on some other user networks. So please use the first set of static routes first and then if needed you can try followings:\
\
Network Address: 23.246.0.0\
Subnet Mask: 255.255.192.0 (or /18)\
Gateway: (use the IP address of your router) \
\
Network Address: 198.38.96.0\
Subnet Mask: 255.255.224.0 (or /19)\
Gateway: (use the IP address of your router)&#x20;

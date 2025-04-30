# Amazon Fire TV

## Register your IP address and choose your prefered Netflix region

1. Login to your client area ([https://wannaflix.com/clientarea.php](https://wannaflix.com/clientarea.php))
2. Click on your active SmartDNS subscription
3. Select your prefered Netflix region and click "Update"

{% hint style="warning" %}
You will have to re-submit your IP address each time it changes (router reboots, new location, etc.)
{% endhint %}



## How to set up Amazon Fire TV

{% hint style="warning" %}
**Update:** With the recent Amazon Fire TV OS update (to Version 5.0.5), Fire TV devices (boxes and sticks) will ignore IPv4 DNS settings in favor of IPv6 if available. Given that IPv6 beaks our service, if you see an IPv6 address for DNS in your device's network settings, then you'll need to disable IPv6 on your router in order to allow your Fire TV to use our DNS.
{% endhint %}

First you need to find the IP of your router. Please use the appropriate method below and note down the IP of your router.

### Find Router IP on Windows

1\. Open up the program command prompt

2\. Type “ipconfig” without the quotes and press enter

3\. The IP address from default gateway is most likely the IP address of your router

### Find Router IP on OS X

1\. Open _System Preferenc&#x65;_&#x73;

2\. Go to _Network_

3\. Click _Advanced_

4\. Go to _TCP/IP_ – here you will see the routers IP

### Change the DNS on the Amazon Fire TV (Wireless)

1. Go to settings
2. Select Systems
3. Select WI-FI
4. Select your WI-FI network and forget WI-FI network by Pressing the button with 3 lines on it.
5. Press the select button.
6. Select your WI-FI network.
7. Enter your WI-FI password and Click on advanced&#x20;
8. Enter the first three groups of numbers exactly the same as the IP address of your router. As an example, if your router IP is 192.168.0.1, then use the IP address 192.168.0.7 or something to that nature. The important part is to change the last digit so you get an IP from the same IP range as the router.&#x20;
9. For the Default gateway enter the IP of your router
10. Input 24 for the Network Prefix Length and Click Next&#x20;
11. Enter **165.227.243.239** for DNS 1
12. Enter **165.227.254.128** for DNS 2

### Change the DNS on the Amazon Fire TV (Wired)

1. Go to Settings
2. Select System
3. Select Network (wired)
4. Select Configure Network
5. Enter a valid IP from your home network. Find the IP of your router in the guides above.
6. Set prefix length to 24. Press Next.
7. Set gateway to the router IP (You can find the correct gateway by following the guides above). Press Next.
8. Set DNS 1 to **165.227.243.239**  Press Next.
9. Set DNS 2 to **165.227.254.128**  Press Next.

### Other Things You Need

* Make sure you have a 1-click US address in your Amazon Account.&#x20;
* Also on Amazon.com go to Your Account > Manage Your Content and Devices > Country Settings and set country to United States

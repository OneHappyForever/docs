# XBOX ONE

## Register your IP address and choose your prefered Netflix region

1. Login to your client area ([https://wannaflix.com/clientarea.php](https://wannaflix.com/clientarea.php))
2. Click on your active SmartDNS subscription
3. Select your prefered Netflix region and click "Update"

{% hint style="warning" %}
You will have to re-submit your IP address each time it changes (router reboots, new location, etc.)
{% endhint %}

## How to Set up Xbox One

1\. __ Go to the _Dashboard_

2\. Press _options_ button the controller

3\. Go to _Network_

4\. Go to _Advanced Settings_

5\. Go to _DNS settings_

6\. Select _Manual_

7\. Enter Primary DNS **165.227.243.239** and press enter

8\. Enter Secondary IP **165.227.254.128** and press enter

9\. Press _B_ for save

10\. Restart the Xbox One

{% hint style="warning" %}
**Important**: There is a known bug on the Xbox One resulting in some users not being able to save DNS settings as the Xbox will revert to 0.0.0.0. We are unable to do anything about this software bug. Please get in touch with the Xbox one support team instead.
{% endhint %}

{% hint style="info" %}
Also make sure that IPv6 is disabled on your router if your ISP supports IPv6.
{% endhint %}

## For Netflix Users

&#x20;In order to use XBOX ONE to access US NETFLIX regions you need Linux based routers like DD-WRT to set NAT rules to reroute all TCP and UDP 53 port traffic to our DNS.\
\
For example:\
\
iptables -t nat -A PREROUTING -p udp --dport 53 -j DNAT --to-destination xxx.xxx.xxx.xxx:53\
iptables -t nat -A PREROUTING -p tcp --dport 53 -j DNAT --to-destination xxx.xxx.xxx.xxx:53\
\
You need to change xxx.xxx.xxx.xxx to one of our DNS servers: **165.227.243.239** or **165.227.254.128**\
\
We know this may be complicated for regular users but this is the only solution at the moment for xbox one devices.\
\
Meantime all our services like Amazon Prime US, Hulu, ABC, BBC, TVPlayer, Zatto, Pandora, etc. are working properly and can be accessed from XBOX devices. Thank you!

# Connection Issues

## Slow connection speed

* Try another server. Some of our servers are optimized for different locations, so choose the one optimized for your country.
* For Chinese users: check [this page](../optimizing-your-vpn.md).
* For Middle Eastern users: Any server in Europe.
* Rebooting your router may help (you will get a fresh IP and clear the router cache).

## Unable to connect to ANY servers

{% hint style="warning" %}
This means no servers can connect. If some are still accessible, see further down below
{% endhint %}

{% hint style="success" %}
How to check if a server is working:

1. Connect to the server
2. Go to [ip.sb ](https://ip.sb)
3. Check that the IP address shown is of the country you connected to

If the IP shown is your local IP, then the server may be working, but the VPN software is not capturing traffic and redirecting it to our servers. Check that the VPN is turned on.
{% endhint %}

Check our telegram group chat for any announcements. If there are none, then usually this is either an account issue or a local issue.&#x20;

* Check your network connection (disconnect from the VPN and go to a site that usually works without VPN). If it that doesn't work, that means it's not the VPN itself that has the issue, but your local internet connection. Try reconnecting to the wifi. If that still doesn't work, restart your computer and your internet router.
* Check that your subscription has not run out/expired. If you switched from the free trial to a paid subscription, you will need to get the new API links from the dashbaord, as the paid subscription is considered a new separate subscription from the free trial and has it's own set of API links.&#x20;
* &#x20;**Make sure you have the latest servers as some will get blocked and will be replaced.** If you added the servers using the api link, you can update the server list via the link (see the guide [here](../faq/updating-the-server-list.md)).&#x20;

#### For v2ray (vmess, aka "old protocol"):

* Check that your computer/phone time is correct and within 90 seconds of the global clock (sync your time via the internet)

**For v2rayN/Netch/Clash on Windows or Mac OS:**

* Check if it's working on another browser (Chome/Edge). If it is, then maybe the browser you are using has a proxy plugin that is interfering with the VPN connection. Try to find it and turn it off.

## Some servers are not working (but others are)

In this case, it could be that the server you are trying to connect to has some issue, or that China's firewall has blocked it.

* Check the status page: [https://status.wannaflix.com](https://status.wannaflix.com) If the server shows as offline, please wait for us to fix it, or send us a message on our telegram group chat.
* If the server shows as online on the status page but is unaccessible to you, first update your server list, as the server details may have been updated.&#x20;
* If that still doesn't work, send us a message in our telegram group chat.

## Website still blocked&#x20;

* Check that you are connected to the VPN (go to [ipx.ac](https://ipx.ac/) to check your IP address)
* If you are using the SmartDNS and a website doesn't work, please open a [support ticket](https://wannaflix.com/submitticket.php?step=2\&deptid=1).

{% hint style="info" %}
This means that only a particular website doesn't work. If **all** websites don't work, refer to the "Can't connect to internet when VPN is connected" section
{% endhint %}

## Netflix still blocked

There may be 2 reasons why Netflix doesn't work. (1) The Netflix app itself, and (2) your VPN settings.

1. The Netflix app:
   * Close/reset the Netflix app
   * Restart your browser
   * Clear browser cookies and cache
   * The Netflix front page and recommended movies no longer changes when switching regions. If movies do play but you believe your region still hasn't changed, try searching for a movie that is in the region you connected to. \
     Alternatively, you can create a new user profile in the Netflix app. Since you are currently connected to that region, the movie list will update to the region you're currently connected to (as it's a brand new profile).
2. Your VPN settings:
   * Check that you are connected to the VPN (go to [ipx.ac](https://ipx.ac/) to check your IP address)
   * If you are using the SmartDNS and a website doesn't work, please open a [support ticket](https://wannaflix.com/submitticket.php?step=2\&deptid=1).

P.S. Make sure that the region you are trying to access is actually supported. We only support US, UK, Canada, Germany, Korea, Japan, Hong Kong, and Singapore Netflix.

## Can't connect to internet when VPN is connected

* Try connecting to another server.
* Check that you have an active internet connection by disconnecting from the VPN and going to normal sites such as [bing.com](http://bing.com)
* Restart your router and modem.
* Make sure your anti-virus or firewall isn't preventing the VPN from connecting to the internet. Disable them for a few minutes and reconnect to the VPN to test. \
  If that is the case, please create an exception for the app in your anti-virus and firewall.

## No internet even after the VPN is disconnected/closed

This is most likely to happen with Clash for Windows and SSR for Windows.&#x20;

The reason for this error is that the traffic capture software that is part of the VPN app is still running and redirecting traffic to your VPN servers, but because the app is closed, it fails.

To solve this, we need to stop the traffic capture software.

### Clash for Windows:

1. Reopen the app.
2. Under "General" uncheck "System Proxy"
3. Now you can Quit the app

### SSR for Windows:

1. Reopen the app
2. Go to Mode > Disable System Proxy
3. Now you can quit the app

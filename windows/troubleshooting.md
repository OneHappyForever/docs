# Troubleshooting

Updated: 11 October, 2020

## My a**nti-virus prevents the app from installing**

1. Remove all traces of the app from your computer \(delete the folder\)
2. Re-download the app again from our website
3. Pause the antivirus software \(recommended for 1 hour or until reboot\)
4. Install the app
5. Create an exception for the app in your anti-virus software

## No internet even after the VPN is disconnected/closed

This is most likely to happen with Clash for Windows, SSR for Windows, and V2rayNG.

The reason for this error is that the traffic capture software that is part of the VPN app is still running and redirecting traffic to your VPN servers, but because the app is closed, it fails.

To solve this, we need to stop the traffic capture software.

### Netch:

1. Reopen the app
2. Click the "Stop" button
3. Now you can quit the app

### V2rayNG:

1. Reopen the app
2. Go to Http Proxy &gt; Not Enabled Http Proxy
3. Now you can quit the app

### Clash for Windows:

1. Reopen the app.
2. Under "General" uncheck "System Proxy"
3. Now you can quit the app

### SSR for Windows:

1. Reopen the app
2. Go to Mode &gt; Disable System Proxy
3. Now you can quit the app

## Some servers are offline

#### If only one or two servers don't work:

It's likely that server has an issue.

* Try a different server \(we usually have several alternatives for important locations like the US and Japan\)
* [Open a support ticket ](https://wannaflix.com/submitticket.php?step=2&deptid=1)letting us know which server\(s\) don't work, or [message us on telegram](https://t.me/wannaflixvpn)

#### If MOST of the server don't work, but a few do:

It's likely your current VPN app is unstable in your location \(probably it's SSTap\)

* Try a different VPN app \(We recommend Netch\)
* Use our \[CHINA\] servers if you are in China

#### If NO servers work:

It's likely either a misconfiguration issue, a local internet issue, or an issue with your account or subscription

**Misconfiguration issue:**

* If you added the servers manually, double check the Port, Password and IP/URL of the server. 
* This is an especially common for OpenWRT routers. Double check that the IP address of that server hasn't changed \(ping the server url again and compare\).
  * If the IP address has changed, then update the IP and reconnect

**Local internet issue:**

* Disconnect from the VPN and check if you can access a normal site \(like [bing.com](https://bing.com)\)
* If you can't, then check your wifi connection. Try reconnecting to your wifi, or rebooting your router

**If it's an issue with your account or subscription:**

* [Open a support ticket](https://wannaflix.com/submitticket.php?step=2&deptid=1)

## SSTap: **All the servers suddenly disappeared**

1. Don't panic. It's likely that the update function failed that one day and the app wasn't able to pull the server list successfully.
2. Click on the cogs icon \(settings icon\)
3. Go to SSR subscriptions &gt; Manual update SSR subscriptions
4. The servers should be back

{% hint style="info" %}
We recommend moving to the newer Netch app as it's much more stable than SSTap.
{% endhint %}


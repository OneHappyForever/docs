# About the Nov. 30 issues + New Servers

## About the Nov. 30 issues

If you live in China, you may have noticed a long outage of some of the \[CHINA\] and Netflix servers yesterday \(Nov. 30\). First of all, we would like to sincerely appologize for the network issues during the day. 

Any downtime is extremely frustrating, and we want you to know we do all we can to make the server as stable as possible.

So, what in the world happened?

Basically, we upgraded our main server's OS version \(aka kernel\), but the new version was unstable and caused the server to crash. 

We had to reroute several \[CHINA\] servers to backups, but the backups were under heavy load so speeds suffered.

We have since reverted back to the older OS version, so the problem is now fixed.

{% hint style="info" %}
We always test new updates on smaller servers before deploying them on to our main servers. This particular update didn't cause any of our test servers to crash, it just so happened to crash the \[CHINA\] main server.

Also, it did not crash the server immediately after installing, but several hours later, perhaps under heavier load.

We've reverted all test servers as well just in case.
{% endhint %}

So, what have we done to prevent such a problem from happening again?

1. We've separated some servers to route to a second datacenter \(see box below\)
2. We're adding additional checks before upgrading or changin server configurations in the future
3. We've added capacity to the backup servers 
4. We have added a backup of a backup \(2 layers\) in case both the main server and the backup fail
5. We've reduced the time it takes to switch to the backup servers from 5 minutes to 1 minute
6. We've added a couple of direct-connect fast servers for the VIP \(note that you can always use our direct-connect server on the normal package as well, just select anyone not labeled as \[CHINA\] or NETFLIX\)

{% hint style="info" %}
Current \[CHINA\] server routing:

Main China Server \(Datacenter \#1\):

* STREAMING
* US NETFLIX 2
* Hong Kong 1 & 2
* Japan 1 & 2
* Korea
* Singapore
* India

Secondary China Server \(Datacenter \#2\):

* Germany 1 & 2
* UK
* France

If the first cluster goes down, please use the second cluster.

We may be adding a third route in the future as well.
{% endhint %}

We are confident that these changes will make the \[CHINA\] servers more stable and resilient going forward.

## NEW Servers

You may have noticed that we have added a few additional servers to the list over the past couple days.

Why?

First, to provide redundancy. Second, to distribute load and improve speeds. We've added a second server cluster to frequently-used locations, including:

* Hong Kong 2
* Japan 2
* Germany 2
* US 2
* New York \(New location!\)

### VIP Improvements

For the VIP servers, we've also added two US servers via CLOUDFLARE CDN for those NOT living in China \(it's too slow for those in China\). This gives up to 2x faster speeds, lower latency, and greatly reduced jitter \(i.e. more stable connections\).

We've also added 2 Hong Kong servers via AMAZON CDN for users in China and abroad. These servers deliver up to 100 Mbps speeds **without going through any China servers.** This means that they won't be affected by downtimes on the China end of things.

And lastly, we've added a Korea server with great pings to China \(50-70ms\) and the rest of the world. This server also does not need to go through any China servers.

To find out more about VIP routing, please [visit this page](../vip-servers/routing.md).

## Last Words

Well in conclusion,  we've got an additional route for \[CHINA\] servers, additional routes to several frequently used locations, plus new VIP servers both for those within and outside China.

We hope that these new changes will give you a better inernet experience no matter where you live or what you use WannaFlix for. 

And with that, until next time!

Happy surfing! :\)

The WannaFlix Team


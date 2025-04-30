# May 2020 Update

## What is this update about?

This update is a complete restructuring of our infrastrure. It aims to:

* Prepare for the next round of blocking between now and mid June
* Implement new V2ray technology to stay ahead of the Great Firewall
* Increase capacity on several key servers
* Provide better stability on the NETFLIX servers
* Simplify the server list
* And other reasons we'll keep to ourselves for now ;)

## What should I do to benefit from the new update?

Update your server list regularly over the next two weeks, up to the beginning of June.

{% hint style="danger" %}
**WE ARE DROPPING SUPPORT FOR CLASH**&#x20;

Clash does not run the official V2ray core. It runs on Clash core instead, which is it's own version of V2ray.&#x20;

**Clash only support a very limited set of options for V2ray.** Going forward, we may need to use more advanced V2ray configurations that will not work with Clash.&#x20;

**Therefore, we are droping support for ALL Clash apps including:**

* **ClashX on MAC**
* **Clash for Windows**
* **ClashA on Android**

These apps may stop working in the future.&#x20;

If you are running any of these apps, please login to your client area dashboard and download the app recommended for your device:

* V2rayU for Mac ([Guide](../installation-guides/mac-os/v2rayu.md))
* V2rayN for Windows ([Guide](../installation-guides/windows/v2rayn-recommended.md))
* V2rayNG for Android ([Guide](../android/v2ray-shadowsocks/v2rayng-recommended.md))

These apps run on the official V2ray-core program and will work.

This is the **last big app change** expected in the next 12 months. We do not expect any major change in protocol or apps until at least May next year (and perhaps longer).
{% endhint %}

{% hint style="info" %}
**We will try our best to maintain backward compatibility for Clash for as long as possible** to allow you and all our users to migrate.

However, depending on how the situation progresses in the future, we may have to break compatibility sooner than expected.

So please migrate as soon as possible!

Thanks!
{% endhint %}

## What if I can't install V2rayU?

For a very very limited set of users (about 1%) on Mac, V2rayU may crash. If so, you can install Qv2ray or [V2rayX](https://github.com/Cenmrev/V2RayX) instead (both run on the official V2ray-core).

## Where have all the CHINA USERS servers gone?

They have been combined with the NETFLIX servers.

They were pointing to the same end servers anyways, so we decided to simplify the server list and combine them.

{% hint style="info" %}
Connect to any NETFLIX server to enjoy the same benefits you got with the CHINA USERS servers.
{% endhint %}

## Which server(s) should I connect to?

{% hint style="warning" %}
Due to the complexity of the Chinese internet, speeds may vary greatly between ISPs and location.

What may work for someone else may not work for you, and what may work for you may not work for someone else.&#x20;

Please **test the servers yourself** to see which ones perform best for you.

These are just **general guidelines** to be used as a starting point.
{% endhint %}

#### For the best speed:

For browsing, downloading, and YouTube streaming.

* Taiwan NETFLIX
* Hong Kong NETFLIX 1 & 2
* Japan NETFLIX
* Singapore NETFLIX
* Singapore load balancers 1-4

#### For the best stability:

Special setup to fight blocking during sensitive times.

* Hong Kong NETFLIX 1 & 2
* Japan NETFLIX
* Taiwan NETFLIX
* Singapore load balancers 1-4

#### For Netflix:

Servers that unblock Netflix.

* The NETFLIX server linked to the region you want to watch

For the fastest Netflix streaming:

* Hong Kong NETFLIX 1 & 2
* US NETFLIX 2
* Japan NETFLIX

## Some servers have stopped working!

It is possible that some of our servers may get blocked in the next month (between now and mid-June, 2020).&#x20;

If that does happen, do not panic. Simply **connect to another server** until we fix the one that got blocked.&#x20;

{% hint style="success" %}
NETFLIX servers are running on special technology and will not get blocked easily.&#x20;

We recommend staying on those servers during the next month for the best stability.
{% endhint %}

## Nothing works, how can I contact you?

If all servers stop working for any reason, please **update your server list first.**

**See** [**how to update your server list.**](../faq/updating-the-server-list.md)

Also, if you are running CLASH (ClashX, Clash for Windows, ClashA), please [see the section about it above](may-2020-update.md#what-should-i-do-to-benefit-from-the-new-update).

If that doesn't work, don't panic! It is likely an issue with your subscription. We're here to help. You can:

* Open a [support ticket](https://wannaflix.net/submitticket.php?step=2\&deptid=1).
* Send us an email at admin@wannaflix.com
* Send us a message on [telegram ](https://t.me/wannaflixvpn)if you can connect to it via a backup VPN

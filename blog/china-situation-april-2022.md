# China Situation - April 2022

Before we start, the entire WannaFlix team would like to express our appreciation for your patience and understanding thoughout the past few weeks.&#x20;

Here at WannaFlix, we value transparency and feel it is your right to know what is going on with the ever-evolving internet situation in China. This will help you understand potential issues that may come up, and changes that we are taking to adapt.

### How WannaFlix keeps your internet fast and secure

First, we need to understand how WannaFlix tunnels your connection out of China.

There are 2 main ways.&#x20;

First, we can encrypt your connection, then wrap it in a TLS layer to make it appear like normal web traffic, and send all of this directly to a server abroad. This is what we do for non-CHINA labeled servers. The protocol is secure and the servers don't get blocked. However, directly connecting to the end servers abroad can be slow.

So the second way is to do the exact same thing, except we first send the traffic to a middle server in China, which has good peering to our end servers abroad. Nothing is decrypted in China so your traffic remains private. But now we also have a fast internet.&#x20;

In previous years, it was our servers abroad that were vulnerable to getting blocked. However, with current protocols, we can effectively evade this kind of censorship. Therefore, it is not a protocol problem.&#x20;

What has been affecting us these past few weeks is blocking of our middle servers in China. This week for example, our servers in China were completely blocked from accessing any website or IP outside of China. This means our middle servers can no longer forward traffic to our end servers, and all CHINA servers went offline.

### How WannaFlix adapts

We have implemented tweaks on the backend to prevent the GFW from identifying our middle servers as proxying foreign traffic.&#x20;

These tweaks require us to only proxy TLS traffic. Therefore, we need to push these updates to our protocol:

* VLESS+XTLS (aka new protocol) will be updated to VLESS+TLS
* VMESS (old protocol) will be updated to VMESS+TLS&#x20;

These changes only require you to update your server list. See [this page.](../faq/updating-the-server-list.md)

As for protocols that don't support TLS, we have setup a different middle server system. This requires the following changes:

* SSR will be changed to SS, and the ports will be moved from 600-607 to 40600-40607
* OpenVPN (Eclipse) http-proxy ports will be moved from 1080-1088 to 41080-41088

SSR changes will only require you to update your server list if you have the API. If you have manually added them into your apps, or if you are running MERLIN routers, you will need to manually add the servers in (MERLIN does not support SS APIs).

The OpenVPN update will require you to re-downlaod the config files. We will announce when you can do so in our telegram group chat (go to your dashboard, and scroll down to the bottom to see it).












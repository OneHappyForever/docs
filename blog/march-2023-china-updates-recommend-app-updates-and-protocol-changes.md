# March 2023 China Updates - Recommend app updates and Protocol changes

#### Summary (tl;dr)

We will be switching our recommended apps to Clash on Windows, Mac OS, and Android. Shadowrocket is still the recommended app on iOS.

Recommended apps:

| OS             | New Recommended App     | Previous Recommended App |
| -------------- | ----------------------- | ------------------------ |
| Windows        | Clash for Windows       | V2rayN                   |
| Mac OS (Intel) | ClashX Pro              | ClashX Pro               |
| Mac OS (M1/M2) | Shadowrocket/ClashX Pro | Shadowrocket             |
| Android        | Clash for Android       | V2rayNG                  |

We will add Shadowsocks support for CHINA servers. Both Trojan and Shadowsocks will co-exist, and users will be able to choose their prefered protocol.

For non-CHINA servers, we will keep the Trojan protocol for the moment.&#x20;

## March 2023 Update

It's been almost a year since our last China update. As the situation in China continues to change, we continue to adapt.

### &#x20;Major changes in the past year

We have notices several major changes in the situation in China.&#x20;

First, since the October meeting last year, datacenters within China have cracked down on VPN traffic. Most of our suppliers closed shop, and new suppliers are unstable. Since then, we have had to change middle servers every few weeks. When a middle server goes down, it will affect the CHINA server being tunneled through it. This has been the main cause of some servers going offline from time to time. To mitigate this issue we are spreading traffic over multiple datacenters.

Second, the Trojan protocol has become unreliable for direct connections. Before the October meeting, Trojan would virtually not be blocked, even when a lot of traffic was going through it. However, the GFW is now blocking Trojan servers from well-known datacenter IP ranges. We now need to obfuscate Trojan before traffic leaves China, and non-China servers are often blocked.

Third, there has been a crackdown on Alipay payments in January and February this year. Some Alipay payment providers have closed shop, or have issues accepting payments. It is not unusual for them to close shop without warning and not pay us. To mitigate this, we are now using 2 Alipay payment gateways. If the first is not working, please try the backup gateway. In case they stop working, we have additional backup gateways ready to launch, so we are well prepared in this regard.

There have been other changes, but these are some of the major changes impacting the China side of things.

We have tried our best to mitigate each issue to provide you with the best service possible.&#x20;

### Other positive changes

There have been positive developments as well.&#x20;

The Clash app is now available on all major platforms except iOS. Clash now supports the TUN packet capturing mechanism, similar to the TAP engine used by OpenVPN. It also supports UWP for proxying Windows App store apps. And it now supports all major protocols except VLESS and XTLS.&#x20;

This means that we now have a single app for all platforms that works well, and that supports all our current protocols.&#x20;

Therefore, **we have decided to simplify our recommended app list to recommend Clash for Windows, Mac OS, Android, and OpenWRT routers.** This will make it easy for you to set things up as you'll have the same look and feel accross platforms. You won't need to re-learn a new app for each platform.&#x20;

Benefits of using Clash:

* Same UI for all platforms (except iOS)
* Supports all our protocols
* The server list is automatically updated  (updates once a day by default)
* Can capture all traffic using the TUN interface
* Supports split-tunneling (you can choose different servers for Web browsing, Netflix, Youtube, etc.)
* UI is well done
* You can add your own rules (for the technically savy)

We will continue to provide APIs for the other apps so if you prefer your current app, you can continue to use it. We try our best to keep backward-compatibility.

### Reintroduction of the Shadowsocks protocol

When we first started providing proxy/vpn services in China, we selected the Shadowsocks protocol. It was fast, stable, and unable to be blocked. At the time, the Trojan protocol did not exist, and v2ray was in it's early stages of development.&#x20;

However, as the GFW evolved, Shadowsocks was becoming unstable, and we adpated by switching to v2ray, then Trojan.&#x20;

It is now time to adapt once again. Since all major protocols are now identifiable by the GFW to a certain extent, including Trojan, we are now using additional obfuscation mechanisms on the China middle servers. This obfuscation works on all protocols, including Shadowsocks.&#x20;

Therefore, since going forward we will have to obfuscate traffic regardless, we are now free to select the best protocol without worrying about it being blocked, at least for connections routed through our China servers.&#x20;

Shadowsocks is lightweight, and support UDP-over-UDP. It doesn't suffer from the TLS or v2ray handshake's additional RTTs (causing slower response times). Some datacenters within China are even more lenient toward Shadowsocks (non-descript TCP/UDP) vs TLS-based protocols.&#x20;

For this reason, we have decided to **re-launch Shadowsocks on our CHINA servers on a trial basis.**&#x20;

If user's feedback is good, we will continue to offer Shadowsocks in China.&#x20;

However, since direct connections on Shadowsocks are easily identifiable, we will continue to offer Trojan only on the non-China servers.&#x20;

Users in other restricted countries will find Trojan better suited for them than Shadowsocks.&#x20;

## Conclusion

Well, that has been an eventful year indeed! We hope that these changes will make your internet experience easier in China.&#x20;

If you have any questions, please feel free to reach out to us via ticket or on telegram.&#x20;

Until next time!

The WannaFlix Team


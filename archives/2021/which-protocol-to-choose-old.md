# Which Protocol to Choose? (old)

{% hint style="danger" %}
Archived and outdated
{% endhint %}

It really depends on where you are located and on what you need.

Let's go through the main pros and cons of each protocol we offer.

## At a Glance...

Recommendation: V2ray for Netflix, Shadowsocks for web-browsing and streaming, Eclipse for security, SmartDNS for TVs and consoles.

|                       | v2ray | <p>Shadow</p><p>socks</p> |        Eclipse       | SmartDNS |
| --------------------- | :---: | :-----------------------: | :------------------: | :------: |
| TCP                   |   ✅   |             ✅             |           ✅          |     ❌    |
| UDP                   |   🟨  |             ✅             |           ✅          |     ❌    |
| ICMP                  |   ❌   |             ❌             |           ✅          |     ❌    |
| Fast                  |   ✅   |             ✅             |          🟧          |    🟨    |
| Stable                |   🟨  |             ✅             |          🟨          |     ✅    |
| Works in China        |   ✅   |             ✅             |           ✅          |     ✅    |
| Unblocks Netflix      |   ✅   |  <p>🟨 </p><p>(Some)</p>  | <p>🟧</p><p>(US)</p> |     ✅    |
| Web-browsing / Email  |   ✅   |             ✅             |           ✅          |     ❌    |
| Video Streaming       |   ✅   |             ✅             |          🟨          |     ❌    |
| Gaming                |   🟧  |             ✅             |          🟥          |     ❌    |
| VoIP/Video Conference |   🟨  |             ✅             |          🟧          |     ❌    |
| Countries             |   15  |            TBA            |           6          |     4    |

{% hint style="info" %}
**GLOSSARY**

_Stability:_ A measurement of the frequency of disconnections and speed fluctuations, as well as the  likelihood of encountering various issues.

_Gaming:_ A measurement of how the protocol performs when gaming. Gaming usually requires good UDP support, stable apps, and low ping (less RTTs).&#x20;
{% endhint %}

## v2ray

V2ray was created on September 5, 2015 as an alternative to Shadowsocks and has slowly gained popularity with users in China (the github repo now has more stars than Shadowsocks). It is more flexible than Shadowsocks, supports multiple protocols out of the box, and can effectively escape blocking by the Great Firewall.&#x20;

V2ray is optimized for TCP only. It only has basic UDP support. v2ray also needs 1 RTT (round-trip time) more than Shadowsocks for it's handshake. You can eliminate this additional RTT by enabling mux support in your apps (however, keep in mind that enabling mux may bring instability in the network and reduce your streaming speed).

Most of our servers run v2ray by default.

#### Use v2ray if:

* You need to watch Netflix or other streaming channels
* You need to connect to a wide variety of countries&#x20;
* You need to connect to a specific country that is only on v2ray
* You want fast downloads and HD YouTube streaming
* Do moderate web-browsing, emails, etc.

**Don't use v2ray if:**

* You need to play online games
* You want to run a UDP-based application
* You need OpenVPN for greater security

## Shadowsocks

Shadowsocks is one of the first protocols developped in China specifically to bypass the GFW. Development started on April 20, 2012. It's original developper was forced to stop his/her work on the project due to outside pressure. Work on the protocol continues on till this day via various forks on the original project.

Shadowsocks was the first protocol we implemented, before we had to switch to v2ray and Eclipse after it was getting aggressively blocked.&#x20;

Unlike v2ray, Shadowsocks is leaner and is easy on RAM and the CPU, making it more stable under load. It has also optimized it's UDP packet transmission mechanism, making it a good option for gaming.

Because Shadowsocks is heavily censored, we need to use various mechanisms to hide the connection. Therefore, only a subset of locations are available for Shadowsocks.

#### Use Shadowsocks if:

* You need a simple, click-and-forget connection
* You do extensive web-browsing, email, streaming, etc.
* You want to play online games (use Netch on Windows)
* You need to do VoIP or video conferencing

**Don't use Shadowsocks if:**

* You want to watch Netflix or unblock streaming content (use v2ray)
* You need a specific country not supported by Shadowsocks
* You are running Linux

## Eclipse (OpenVPN)

Eclipse is our own version of OpenVPN, modified to work in China. It has never been blocked, nor do we see it getting blocked in the near future. It runs on the official OpenVPN apps, and support all the functions of OpenVPN.

It uses 256-bit encryption, supports TCP, UDP, and ICMP protocols, and is thoroughly audited by industry experts to guarantee strong security.

The main downside of Eclipse is that it is slow. Speeds are usually between 3-12Mbps depending on the time of day and server choice (though you may get speeds of up to 25Mbps on some networks).

#### Use Eclipse if:

* You want an industry-standard VPN solution
* You need military-grade security&#x20;
* You are doing light browsing, emails, streaming, etc (Eclipse can stream 720p HD)
* You need support for ICMP or other non-standard protocols
* You need Linux support

**Don't use Eclipse if:**

* You want a fast connection

## SmartDNS

SmartDNS is a DNS server that unblocks Netflix and other streaming channels for you. You need to register your IP for authentication and add the DNS servers into your WiFi/ethernet settings and your good to go!

NOTE: It does NOT encrypt your connection. It does NOT bypass DNS poisoning by ISPs. It does NOT bypass China's firewall. It does NOT unblock Youtube.

It only bypasses geolocation blocking by Netflix and other such streaming channels.

#### Use SmartDNS if:

* You want to watch Netflix or a similar channel on a device that does not support v2ray (smart TV, console, etc)
* You want to only unblock Netflix, but don't need a VPN to bypass your local internet restrictions (i.e. you don't live in China)

**Don't use SmartDNS if:**

* You need to bypass your ISP/School/Country's firewall
* Your ISP is doing DNS poisoning/hyjacking on the domains you want to unblock
* You want a VPN
* You have v2ray/Shadowsocks/Eclipse running at the same time (they will conflict with each other)

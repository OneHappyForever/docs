# Switching to the New Protocol

### A little history

What do we mean by old and new protocol? We are refering to older and newer v2ray implementations.&#x20;

We started using the older VMESS on TCP protocol in 2019 after Shadowsocks was getting blocked quite effectively by the GFW (great firewall). At the time it wasn't easily blocked by the firewall and served us well.&#x20;

However, the old protocol had some shortcomings, such as a poor UDP support, additional RTTs (round-trip time), and heavier CPU usage due to multiple encryptions (often resulting in the same packet being encrypted 3 times).

&#x20;The new protocol was developed in late 2020 and beginning of 2021. It uses a new protocol called VLESS, which is leaner. Instead of implementing it's own encryption, VLESS uses TLS. The new protocol has faster speeds, less RTTs, good UDP support, and is extremely resistant to blocking by the GFW.&#x20;

TO BE CONTINUED...

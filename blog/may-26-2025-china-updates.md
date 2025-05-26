# May 26, 2025 China Updates

Dear users,

It has been over 2 years since our last major China update. During the last update, we had re-introduced the Shadowsocks protocol and updated our recommended apps.&#x20;

Since then, the situation in China has stabilized a lot and we have not had any major issues in the past 2 years, including during sensitive periods.&#x20;

During that time, Shadowsocks has become our Chinese users' preferred protocol, being used more than twice as much (in total data usage) as v2ray and Trojan combined.&#x20;

It seems that Shadowsocks is once again the better option for China as of 2025.&#x20;

**Therefore, we have decided to retain Shadowsocks as the main China protocol going forward, and phase out v2ray starting June 1, 2025.**

### **Why the change?**

As pointed out in our March 2023 update, Shadowsocks has several benefits over v2ray and Trojan:

* Uses less CPU/RAM, and provides better battery life
* Support UDP-over-UDP. This means better experience on apps that use UDP, like gaming and VoIP (Whatsapp calls, Zoom, etc). V2ray/Trojan only supports UDP-over-TCP, which causes lags
* Doesn't suffer from the TLS or v2ray handshake's additional RTTs. Each additional RTT results in a general slower internet experience.
* Some ISPs within China are even more lenient toward Shadowsocks (non-descript TCP/UDP) than TLS-based protocols.

In addition, consolidating the server list around the best protocol has advantages of its own:

* Shorter server list for you (no need to scroll too much)
* Less confusion (Why are there 2 copies of the exact same CHINA servers? What is the difference?)
* Less bugs (Instead of troubleshooting 2 protocols, we just need to troubleshoot 1, which also means we are more focused on ironing out bugs on the one protocol)
* Better apps (Instead ofbeing forced to choose apps that support ALL protocols simultaneously, we can use apps that provides the best experience for that one protocol)
* Easier troubleshooting (includes faster turn around times when servers have issues)
* Less server maintenance overhead (we just need to maintain one set of servers). This frees up time to continue to improve our service in other ways

Among many other benefits.&#x20;

These are just some of the reasons we have decided to remove the v2ray server protocol from the server list starting June 1, 2025.

### What do I need to do?&#x20;

The short answer is nothing. The new server list will appear automatically on June 1 in your apps. If it does not, you can simply update the server list from the API link manually (see [this guide](../faq/updating-the-server-list.md)).&#x20;

All servers currently available will still be there! Just on the Shadowsocks.

### **What about Trojan?**

The Trojan protocol will still remain part of our service, as it is still effective in countries outside China.&#x20;

In addition, if ever Shadowsocks encounters issues in China in the future, we will still have another protocol that we can quickly switch to if needed.&#x20;

### Conclusion

We hope this short explanation of why we are making these changes has helped clarify things. We hope that these changes will make your internet experience smoother in China.&#x20;

If you have any questions, please feel free to reach out to us via ticket or on telegram.&#x20;

Happy surfing!

The WannaFlix Team




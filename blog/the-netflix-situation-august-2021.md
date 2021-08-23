# The Netflix Situation - August 2021

### TL;DR \(aka. short version\)

Netflix has updated its algorithm. Most regions can no longer unblock Netflix reliably. We believe we will be able to continue to unblock US, Japan, and Hong Kong regions going forward without too much difficulty. As for the other regions, we will continue to try to keep them unblocked, but we cannot provide any guarantees at this time.

NOTE: This does not affect any other streaming services like Hulu, Disney+, etc.

### Long version:

On August 4, 2021, Netflix drastically changed its VPN detection algorithm. Most VPNs were no longer able to unblock Netflix, including the largest ones such as ExpressVPN and NordVPN. This new update was so extreme that some users who were not using VPNs in the US had their home IPs blocked by Netflix. 

Clearly, this was a change in Netflix's blocking strategy. Why did Netflix make this change? And how will it affect Netflix-unblocking services in the future, including WannaFlix? Let us see.

### Why Netflix blocks VPNs

To understand how the latest round of blocking will affect us, we need to understand the reasons behind it. 

Netflix itself actually does not want to block VPNs. In fact, even when Netflix identifies a connection as coming from a VPN server, it still allows you to watch shows it has produced in-house. After all, it doesn't cost anything to let you watch them, and Netflix can keep you on its platform.

The problem appears when Netflix has to buy the rights to offer movies and TV shows owned by other companies, like Disney, Universal Pictures, etc. Usually these companies only give Netflix the rights to show their content in some countries, and they put pressure on Netflix to block access to customers who don't live in those countries \(aka, those using VPNs\).

Bottom line: Netflix wasn't trying very hard to block VPNs before. But it seems the networks have increased their pressure, and Netflix had to update its algorithm as a result.

### How most companies used to unblock Netflix before the update

As we have seen, Netflix wasn't trying very hard to block VPNs. It most likely relied on a list of datacenter IP addresses either built in-house or bought from a third party, which was only rarely updated. 

This meant that many datacenters would still work with Netflix as long as the IP wasn't part of well-known datacenter ranges. 

Most VPNs would just use datacenter IPs directly, as it was easy to purchase a large amount of them. In addition, running a server in a datacenter guaranteed the best speeds.

### How Netflix is currently blocking VPNs

However, Netflix has now changed it's blocking model from a blacklist to a dynamic algorithm \(similar to the GFW\). It can quickly identify VPN connections and can block specific IPs within a few hours. 

In fact, as mentioned before, it even blocks residential IPs of home users, which means VPNs can't even rely on truly residential IPs either \(i.e. running a server inside someone's home instead of in a datacenter\).

In our opinion, it seems likely that Netflix is looking at a variety of factors, including how many connections are coming from a single IP.

Now you can understand why even the largest VPNs with large teams and a lot of resources still have not found a solution.

### What can be done?

There are several ways to bypass Netflix's algorithm, but they are not easy to implement. We are still experimenting with what works best, and what is most reliable. 

This is why it took us 2-3 weeks before writing this post. We wanted to gather enough information to make an informed assessment of the situation and what we could reasonably offer. We did not want to make empty promises, or offer something that would stop working a couple of days later.

This is what we have found:

* It is no longer possible to guarantee with any degree of certainty the unblocking of Netflix in any region other than the US, Japan, and Hong Kong
* We may still be able to unblock these regions occasionally \(but we realize occasionally is probably not good enough as you need to be able to watch your shows when you want to, not hit-or-miss\): Germany, Taiwan, Canada
* We currently have no reliable way to unblock UK and Korea Netflix

{% hint style="warning" %}
You may have noticed that 2 of our main regions are now unable to unblock Netflix: UK and Korea.

We know Korea is an important region for some of you Korean expats. We are still trying to find a solution, but to be perfectly honest: we are not very hopeful.
{% endhint %}

### Recommendations and looking ahead

Here is what we recommend:

If you are only interested in Japan, Hong Kong, or US Netflix, everything should be fine. Especially in the US, we can reliably unblock it right now.

We are still working for Netflix's original shows, connecting to those regions will let you watch them in those languages \(Korean, etc.\). If you need to watch the other part of the catalog in those regions, and this is the only reason why you are using us, you may need to consider other options. Just one word of advice: almost all VPNs currently do not work with Korea or UK at the moment, so just be careful not to lose your time and money when searching for an alternative. 

It may be a better option to try another streaming service other than Netflix. We are still working just fine with all the other streaming providers like Hulu, Disney+, Amazon Prime, etc. Check that they have the shows you want in advance.

{% hint style="info" %}
NOTE: These recommendations are for the current situation. If Netflix updates it's algorithm again or if we find a way to unblock additional regions, these recommendations may change in the future.
{% endhint %}

The internet situation is constantly changing; what we can do is adapt. 

We hope this post has clarified some things regarding the current Netflix situation, and what can be expected in the future. 

If you have any questions, please feel free to let us know by ticket or on our telegram group chat. We're always here to help.


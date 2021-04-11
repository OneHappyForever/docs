# Proxifier 4.05

{% hint style="info" %}
What is proxifier: 

Proxifier captures all TCP traffic from your computer and forces it through the local v2ray/SSR app. 

The Portable Edition only captures traffic from apps with a graphical user interface, but the Standard Edition captures traffic from all sources. 
{% endhint %}

{% hint style="info" %}
Why is it useful?

In conjuction with the v2rayN, v2rayU, or Netch under Proxy mode \(TUN/TAP mode will conflict with Proxifier\), you can get all apps to work through WannaFlix.
{% endhint %}

## Installation:

Go to the Proxifier website and download the latest version for your Windows or Mac computer.

[https://proxifier.com/download/](https://proxifier.com/download/)

Run the installer. When it asks you for your registration keys, enter ULTRAVPNS as the username and the following as key:

L6Z8A-XY2J4-BTZ3P-ZZ7DF-A2Q9C（Portable Edition\)

5EZ8G-C3WL5-B56YG-SCXM9-6QZAP（Standard Edition）

P427L-9Y552-5433E-8DSR3-58Z68（Mac OS） 

## Connect it with your v2rayN/Netch/V2rayU/Clash apps

Open the Proxifier app. Go to Profile &gt; Proxy servers &gt; Add.

For the IP, type: 127.0.0.1

For the Port, type the port that the v2rayN/Netch/V2rayU/Clash app is listening on. You can find it in the app settings.

{% hint style="info" %}
Default ports:

V2rayN: 10808

Netch: 2801

SSR: 1080

Mac V2rayU: 1086
{% endhint %}

For the Protocol, select SOCKS version 5.

Leave the credentials blank.

{% hint style="warning" %}
**Important:** Do **NOT** turn your apps on. They are already listening on the local ports by default. Just make sure they are running, but no need to connect to a server. 

The only exception to the rule is Netch, which needs to be run on the Non-system proxy mode.
{% endhint %}


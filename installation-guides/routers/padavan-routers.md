# Padavan Routers

{% hint style="danger" %}
**We do NOT guarantee that our VPN will work with your specific router.** 

Each router is different. The same model may be flashed with a different version of the OS, and some routers may only support older OS versions which don't work with our App.
{% endhint %}

## Recommended routers

We have tested our software with these routers:

### On TaoBao:

 [友华WR1200JS MT7621A千兆1200M路由器 双频AC无线带USB 刷好系统 ](https://item.taobao.com/item.htm?spm=a230r.1.0.0.6cc2e18a0bXRdS&id=582244748555&ns=1#detail)  
[路由宝 L2 双频千兆 AC1200无线路由器潘多拉PADAVAN MT7621A](https://item.taobao.com/item.htm?spm=a230r.1.14.16.d53c59a0BcuijF&id=581908274636&ns=1&abbucket=16#detail)

The routers above come pre-installed with all the software you need. No need to flash anything.

{% hint style="info" %}
We only guarantee this guide will work with the routers above
{% endhint %}

## **Step 1: Log into your Padavan router**

1. Connect to your router's WiFi
2. Open your browser on your computer and type 192.168.123.1 \(may be different for your router, check the bottom of your router  for the actual details\) on the url bar
3. Enter your username and password to login to the router's control panel \(if it's the first time, the username and password are usually both 'admin'\)

## **Step 2: Copy your subscribe link**

1. Login to your client area \([https://wannaflix.com/clientarea.php](https://wannaflix.com/clientarea.php)\)
2. Click on "Manage your VPN Subscription" under 'Your Subscription'
3. Under the box "Your Subscribe Links", click on the "Subscribe Link" button to copy your link to the clipboard

## **Step 3: Paste your subscribe link**

1. On the menu bar on the left of your Padavan control panel, go to "Shadowsocks"
2. On the top bar of the Shadowsocks panel, click on "节点配置" or "Shadowsocks Server" \(depending on the language installed\)
3. Paste the Subscribe link into the box next to "ssr\_服务器订阅" and click on the light blue button next to it \(labelled "更新"\) to download the server list

{% hint style="info" %}
If you don't have that option, then you'll have to enter the servers manually on the first tab.
{% endhint %}

## **Step 4: Choose your server**

1. Choose the server you'd like to connect to from the list \(tick the box next to it\)
2. Scroll down and click on the green button labelled "应用主SS" to set it as the main server
3. Select a backup server from the list, scroll down and click on the second green button labelled "应用备SS" to add it as a backup server \(in case the main one is down\)
4. Click the blue "Apply" button

{% hint style="info" %}
If you had to enter the servers manually, you can skip this part.
{% endhint %}

## **Step 5: Connect**

1. Scroll back up and change the options to match the one in the picture below
2. Click "Apply"
3. If you haven't done so already, toggle the switch on \(as in the picture above\) and click "Apply" to connect

{% hint style="info" %}
To switch servers, simply select another one from the list and set it as the main server by clicking on the "应用主SS" button. Then click "Apply". Finally, scroll back up, toggle the switch off, click "Apply", and toggle the switch back on and click "Apply" to disconnect from the old server and reconnect to the new one.
{% endhint %}






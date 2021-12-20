# Passwall

{% hint style="info" %}
Many third-party modded OpenWRT designed for the Chinese market are pre-installed with Passwall.&#x20;

To see if your router will be installed with Passwall, please contact your router provider before buying it.
{% endhint %}

{% hint style="warning" %}
We only provide instructions on how to setup Passwall with WannaFlix. We do not provide instructions on how to install Passwall on your router if it isn't already installed.
{% endhint %}

## Add your API link

1. Login to your client area dashboard
2. Go to Setup for Router > OpenWRT Passwall
3. Click "Copy the API"
4. Login to your router and open your Passwall app

![](../../.gitbook/assets/image\_1gpnm4i.png)

5\. Go to the Subscribe/节点订阅 tab

6\. Click Add/添加 and paste the API in the URL box

7\. Tick the box to enable the API&#x20;

8\. Click Save & Activate/保存&应用

![](../../.gitbook/assets/image\_51nknf.png)

9\. Click Manually update server list/手动订阅 to pull the servers from the API

![](../../.gitbook/assets/image\_d3w3xz.png)

#### Automatically update the server list everyday

1. Tick Enable automatic update/开启自动更新订阅
2. Click Save & Activate/保存&应用

![](../../.gitbook/assets/image\_1bvrp2e.png)

## Connect

1. Go to the Basic Config/基本设置 tab (it's the first one)
2. Tick the "Enable" option
3. Select the server from the drop down menu&#x20;
4. For UDP and Socks option, set it to connect to the same one as the TCP server

![](../../.gitbook/assets/image\_1ku4a2u.png)

5\. Leave the rest of the options as they are

6\. Click Save & Activate/保存&应用

![](../../.gitbook/assets/image\_9wbhyt.png)

You should be connected

# V2ray

## Disclaimer

{% hint style="danger" %}
**We do NOT guarantee that our VPN will work with your specific router.**&#x20;

Each router is different. The same model may be flashed with a different version of the OS, and some routers may only support older OS versions which don't work with our App.

Please only purchase a router listed in this guide below.&#x20;
{% endhint %}

{% hint style="danger" %}
**We do NOT provide extensive customer support for routers.**

We only support routers listed in this guide below.

We only provide support for **configuration** of the V2ray app:

* Where to put the API link and how to update it.
* How to setup DNS to prevent DNS poisoning.
* How to connect to a specific server.

We do NOT provide ticket support for:

* Flashing your router
* Installing the V2ray app on the router&#x20;
* Exception: If links in this guide are no longer working, you can open a ticket with us to get working links.

However, we do provide this guide in English, as well as links to other resources you can read should you need more info.
{% endhint %}

{% hint style="danger" %}
**We only support Merlin-Koolshare NOT Vanilla Merlin**

You'll need to **flash your router** with one of the firmwares in the links in this guide below.
{% endhint %}

{% hint style="info" %}
Additional resources:

[~~FancySS Github~~](https://github.com/hq450/fancyss) ~~- V2ray app repository, links to Merlin-Koolshare download locations \[OUTDATED, DOES NOT WORK]~~

[V2ray\_bin Github](https://github.com/cary-sas/v2ray\_bin) - Latest v2ray app repository for Merlin Koolshare 380

[Merlin Clash Docs ](https://mcreadme.gitbook.io/mc/)- Clash for Merlin, for those with Merlin Koolshare 384 and 286

[Merlin-Koolshare kernels](https://fw.koolcenter.com) - All available Merlin-Koolshare kernel downloads
{% endhint %}

Alright! With that out of the way, let's get started!

## Buying Your Router

The v2ray app for Merlin is part of the fancyss app package. It can only be run on a customized version of Merlin, Merlin-Koolshare.

Therefore, you'll need to get a router that can be flashed with Merlin-Koolshare (or that comes with it pre-installed).&#x20;

{% hint style="info" %}
#### Overview:

1. Purchase a router that can run Merlin-koolshare
2. Flash it with Merlin-Koolshare
3. Download and install the FancySS app package
{% endhint %}

### Routers

{% hint style="warning" %}
Please only purchase routers listed below
{% endhint %}

**Running Fancyss\_hnd:**&#x20;

&#x20;     ASUS routers: `RT-AC86U` `GT-AC5300` `RT-AX88U` `GT-AX11000`&#x20;

&#x20;    Other routers: `NETGEAR RAX80`&#x20;

**Running Fancyss\_arm384:**

&#x20;     ASUS routers: `RT-AC68U` `RT-AC66U-B1` `RT-AC1900P` `RT-AC87U` `RT-AC88U`  `RT-AC3100` `RT-AC3200` `RT-AC5300`&#x20;

**Running Fancyss\_arm:**

NOTE: This version of Fancyss is no longer maintained and will not receive updates. **Only get a router from this list if you're on a budget.**

&#x20;    ASUS routers: `RT-AC56U` `RT-AC68U` `RT-AC66U-B1` `RT-AC1900P` `RT-AC87U` `RT-AC88U` `RT-AC3100` `RT-AC3200` `RT-AC5300`

&#x20;    NETGEAR routers:  `R6300V2` `R6400` `R6900` `R7000` `R8000` `R8500`

&#x20;    LinksysEA routers:  `EA6200` `EA6400` `EA6500v2` `EA6700` `EA6900`

&#x20;    HuaWei routers: `WS880`

{% hint style="danger" %}
If you don't have a router listed here, please do NOT continue with the guide. It will not work.
{% endhint %}

## Flashing your router

Once you've bought your router, you'll need to flash it with Merlin-Koolshare.

### Preparations

1. Make sure you already have Merlin flashed on your device
2. It is recommended to first update your Merlin firmware to the latest version from your router's manufacturer website or merlin's website before installing KoolShare.

### Download the KoolShare firmware

Find which version of Fancyss your router supports from the router list above.

#### For **Fancyss\_hnd:**

* [ASUS RT-AC86U merlin改版固件](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_386/RT-AC68U/)
* [ASUS RT-AC86U 官改固件](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_386/RT-AC86U/)
* [ASUS GT-AC5300 官改固件](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_386/RT-AC5300/)
* [ASUS RT-AX88U merlin改版固件](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_386/RT-AX88U/)
* [ASUS GT-AX11000 官改固件](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_386/GT-AX11000/)
* [NETGEAR RAX80 梅林改版固件](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_386/Netgear/RAX80/)



#### **For Fancyss\_arm384:**

[https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_384/](https://fw.koolcenter.com/Koolshare\_RMerl\_New\_Gen\_384/)

#### **For Fancyss\_arm:**

[https://fw.koolcenter.com/Koolshare\_Merlin\_Legacy\_380/](https://fw.koolcenter.com/Koolshare\_Merlin\_Legacy\_380/)

{% hint style="info" %}
For EA6200 router, download the latest 7.9.1 firmware [here](https://wannaflix.com/dl.php?type=d\&id=23).&#x20;
{% endhint %}

### Flash your router with KoolShare <a href="#flash-your-router-with-koolshare" id="flash-your-router-with-koolshare"></a>

1. Login to your Merlin router
2. Go to Administration > Firmware upgrade
3. Click on "Choose file"
4. Find your downloaded firmware (ends in .trx) and click "Upload"

![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4Ur6UoV6PAmnnP4mG%2F-Lc4\_Qd3i-GJyOM7-TRW%2Fmerlin-uploadFile.png?alt=media\&token=c4363d77-1af8-468c-8422-2e197e347d59)

## **Enable JFFS** <a href="#enable-jffs" id="enable-jffs"></a>

Next, we need to enable JFFS to be able to upload FancySS to our router.

1. Go to Administration > System
2. Enable "Enable JFFS partition", "Format JFFS partition at next boot", and "Enable JFFS custom scripts and configs"
3. Click "Apply" at the bottom of the page
4. Reboot your router

![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4Ur6UoV6PAmnnP4mG%2F-Lc4bzrI3ih1wFmAAu61%2Fmerlin-JFFS.png?alt=media\&token=ca97455d-f49d-4286-b43d-c0c06240a559)

## Install the APP (FancySS) <a href="#install-the-app" id="install-the-app"></a>

First, you need to download the correct version of FancySS for your router.&#x20;

Go to the corresponding page below and download the latest version of the shadowsocks.tar.gz file.&#x20;

The file will have a version number. You'll need to **rename** it to just **shadowsocks.tar.gz**

#### For Merlin Koolshare 380

{% embed url="https://github.com/cary-sas/v2ray_bin/releases" %}

#### For Merlin Koolshare 384/386

Use Merlin Clash instead:

{% embed url="https://mcreadme.gitbook.io/mc" %}

{% hint style="warning" %}
**IMPORTANT**

**Once downloaded, you have to rename the file to shadowsocks.tar.gz**
{% endhint %}

### Install Shadowsocks.tar.gz on your router

1. Login to your router
2. Go to "软件中心" on the left menu
3. Click on the "离线安装" tab at the top (see picture)
4. Click on "Choose File" and select the \[shadowsocks.tar.gz] file you downloaded in step 1
5. Click on "上传并安装"

![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4kF0Z2i5WU51BNVBu%2F-Lc4llOuwDXNwqOVdoa2%2Fmerlin-installSSR.png?alt=media\&token=a3ee4696-a055-4762-bbb6-5e7362ccd25f)

{% hint style="warning" %}
If you get an error message saying that the package is not allowed to be installed, you need to remove the restriction.

1. Enable SSH in Administration > System
2. SSH into your router (you can use [putty ](https://www.putty.org)on windows, or terminal on Mac) and run the following command:

sed -i 's/\tdetect\_package/\t# detect\_package/g' /koolshare/scripts/ks\_tat\_install.sh

That is one line only.

See [https://hq450.github.io/fancyss/](https://hq450.github.io/fancyss/)
{% endhint %}

## Add Your Servers <a href="#add-your-servers" id="add-your-servers"></a>

### Copy your subscribe link <a href="#copy-your-subscribe-link" id="copy-your-subscribe-link"></a>

1. Go to your [client area](https://wannaflix.com/clientarea.php) dashboard
2. Select "Router" > "Merlin" as your device type
3. Choose "V2ray" as your VPN type
4. Copy the api link provided

{% hint style="info" %}
If you are using Merlin Clash, get the Clash API from Clash for Windows in the Windows APIs on your dashboard
{% endhint %}

### Add your servers <a href="#add-your-servers-1" id="add-your-servers-1"></a>

1. Login to your router
2. Go to "软件中心" on the left menu
3. Scroll down and click on the paper airplane icon (see picture)

![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4kF0Z2i5WU51BNVBu%2F-Lc4psZtScfObvcYhnf8%2Fmerlin-open-ssr.png?alt=media\&token=8b16eb56-0caf-41d1-af3f-6a2017ebc65e)

4\. A popup will appear. Click on "订阅节点" (the button in the middle)![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4kF0Z2i5WU51BNVBu%2F-Lc4p5y\_EEmSxo1N7cHm%2Fmerlin-addsubscribe.png?alt=media\&token=7683c716-6538-401c-ac43-ae6c0c2eda96)

5\. Scroll down and paste your Subscribe Link in the box (see pic)

6\. Set all the settings according to the picture below

7\. Finally, click "保存并订阅"![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4kF0Z2i5WU51BNVBu%2F-Lc4pUog\_SF5zE4agOdq%2Fmerlin-subscribe.png?alt=media\&token=696974be-22de-4c2e-8274-ea16cf6e2c5f)

## Connect to the VPN <a href="#connect-to-the-vpn" id="connect-to-the-vpn"></a>

1. Select a server from the drop-down menu
2. Toggle the switch at the top of the screen (see picture)
3. Scroll down to the bottom and click "保存&引用"

![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4kF0Z2i5WU51BNVBu%2F-Lc4rPHxmEs7TKUxLcho%2Fmerlin-connect.png?alt=media\&token=9874fbe3-b9f1-41f3-ba35-ab3dbeb78adc)![](https://gblobscdn.gitbook.com/assets%2F-Lc04095R6CkPoB8xaCl%2F-Lc4kF0Z2i5WU51BNVBu%2F-Lc4rS1EPOWFNrB\_m5jh%2Fmerlin-save.png?alt=media\&token=690e7fcd-712a-4ff0-9a92-f19a6b7666e5)

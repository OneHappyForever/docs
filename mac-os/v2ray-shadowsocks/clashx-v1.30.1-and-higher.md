# ClashX v1.30.1 and Higher

Updated: August 5, 2022

{% hint style="info" %}
**IMPORTANT**

**We no longer support versions under 1.30.1. Please update to the latest version if you are running a version older than 1.30.1.**
{% endhint %}

{% hint style="warning" %}
**If you have an M1 Mac, we recommend using** [**Shadowrocket**](shadowrocket-m1-macs-only.md) **instead.**
{% endhint %}

## Watch Tutorial Video:

We highly recommend watching the video tutorial. You can stream it in China too.

[Video](https://watch.cloudflarestream.com/5ceac0d642744c812af04af1942cc332)

## Download and install

[Click here](https://wannaflix.com/dl.php?type=d\&id=41) to download the app, then run to install. ****&#x20;

{% hint style="info" %}
Version: 1.95.0.1

Released: July 13, 2022

Native M1 Mac support
{% endhint %}

{% hint style="success" %}
Alternative mirrors:

Download via [App Center](https://install.appcenter.ms/users/clashx/apps/clashx-pro/distribution\_groups/public) (ClashX PRO v1.72.0 and up)

Download on [Github](https://github.com/yichengchen/clashX/releases/download/1.20.0/ClashX.dmg) (version 1.30.1 and up)
{% endhint %}

If it is the first time using ClashX, a pop up will appear saying that the app is from an unknown developer. You need to allow this app to open.

The first time ClashX runs, you will be prompted to install a plugin. This plugin is used to set up the system proxy, otherwise you will need to enter your administrator password each time you connect to the VPN. Click "Install" and macOS will prompt for the user password.

![](<../../.gitbook/assets/Screen Shot 2022-08-05 at 6.32.51 PM.png>)

## Add the servers

### Get the api link

1. Go to your [client area](https://wannaflix.com/clientarea.php) dashboard
2. Click on the dropdown menu under "Setup for Mac OS" and select ClashX for MacOS
3. Click "Copy full API" to copy the API to your Clipboard

### Paste the API

1. After running ClashX, click the Clash icon (a kitten) on the menu bar, and then click Config > Remote Config > Manage in the menu.

![](<../../.gitbook/assets/Screen Shot 2022-08-05 at 8.04.24 PM.png>)

2\. A new window will open. Click "Add", paste your Clash API link and click OK.

![](<../../.gitbook/assets/Screen Shot 2022-08-05 at 8.00.15 PM.png>) ![](<../../.gitbook/assets/Screen Shot 2022-08-05 at 8.02.22 PM.png>)

If you have pasted the correct link and the network is properly connected to the Wannaflix API, you should see a success message.

![](../../.gitbook/assets/5d5c4570d5f092b49ab5137e92550bdc.png)

{% hint style="info" %}
If you do not see this message, check that you have an internet connection and an active subscription.&#x20;

You can also try to manually update it by going to Config > remote config> update
{% endhint %}

{% hint style="success" %}
**RECCOMENDATION:** Set the subscription to auto update by going to Config > remote config > auto update
{% endhint %}

## Start the VPN

1. Select Proxy Mode : (Global)
2. Under GLOBAL, chose a server from the list
3. Check "Set as system proxy" to enable ClashX and connect to Wannaflix.&#x20;

![](<../../.gitbook/assets/Screen Shot 2022-08-05 at 8.12.32 PM.png>)

You can select the server by clicking on Global and selecting a server from the list.&#x20;

{% hint style="info" %}
We also recommend to check "Start at login" to automatically launch the ClashX application at boot time.
{% endhint %}

{% hint style="success" %}
If you are using ClashX **Pro**, you can enable "Enhanced Mode" in the dropdown menu for better stability (i.e. app support).
{% endhint %}

## If you already have ClashX

Please re-download the app from the link above. It's an updated version. Older versions may not work.

After updating from the old version of Clash to the new version, you may see the following error:

![](../../.gitbook/assets/378125d64dc2b271c9b1cafc42fdd634.png)

This is a known bug with the current version of clash. It's not related to the Wannaflix configuration API.&#x20;

To solve this, click the ClashX icon in the status bar and select "Configure" - "Open Configuration Folder".

Delete the config.yaml file in the open Finder window.

![](../../.gitbook/assets/f2156562aac93e23b2730837ecbbc05c.png)

Then exit and restart the ClashX application.

## Troubleshooting

To be done...

Please submit your issues to our telegram group chat. We will update this section with the most common issues.


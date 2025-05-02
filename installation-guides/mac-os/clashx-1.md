# ClashX v1.20 (deprecated)

{% hint style="danger" %}
**IMPORTANT**

**We will be dropping support for ClashX versions lower than 1.30.1 by August 20, 2020. Please update to the latest version now!**
{% endhint %}

{% tabs %}
{% tab title="Go to Clash v1.30.1 and up" %}
[ClashX v1.30.1 and Higher >](clashx-v1.30.1-and-higher.md)
{% endtab %}

{% tab title="Show me the old guide" %}
## Download and install

[Click here](https://wannaflix.com/dl.php?type=d\&id=18) to download the app, then run to install.

{% hint style="success" %}
Alternative mirrors:

Download on [Github](https://github.com/yichengchen/clashX/releases/download/1.20.0/ClashX.dmg) (version 1.20.0)
{% endhint %}

If it is the first time using ClashX, a pop up will appear saying that the app is from an unknown developer. You  need to allow this app to open.

The first time ClashX runs, you will be prompted to install a plugin. This plugin is used to set up the system proxy, otherwise you will need to enter your administrator password each time you connect to the VPN. Click "Install" and macOS will prompt for the user password.

![](<../../.gitbook/assets/27ea88123713c4a37330dadc0a60d44f (1).png>)

## Add the servers

### Get the api link

1. Go to your [client area](https://wannaflix.com/clientarea.php) dashboard
2. Select "Mac OS" as your device type
3. Choose "V2ray" as your VPN type
4. Copy the link provided
5. After running ClashX, click the Clash icon (a kitten) on the menu bar, and then click “Config – Remote Config – Set Url” in the menu.

![](../../.gitbook/assets/41d698ed0cee3d62af6d1fc6d94a81fa.png)

{% hint style="warning" %}
If you are running an updated version of ClashX, the menu names may be different.&#x20;

In that case, go to Config > Remote Config > Manage, and paste the URL there.
{% endhint %}

6\. A new window will open. Paste your Clash API link and click OK.

If you have pasted the correct link and the network is properly connected to the Wannaflix API, you should see a success message.

![](../../.gitbook/assets/5d5c4570d5f092b49ab5137e92550bdc.png)

## Start the VPN

1. Select Proxy (or "Wannaflix" depending on your app version)
2. Chose a server that starts with "V2ray"

Check "Set as system proxy" to enable ClashX and connect to Wannaflix. You can select the server by clicking on Wannaflix and selecting a server from the list.&#x20;

We also recommend to check "Start at login" to automatically launch the ClashX application at boot time.

![](../../.gitbook/assets/7eba10589f970b06c993d3aa6275200a.png)

## If you already have ClashX

Please re-download the app from the link above. It's an updated version. Older versions may not work.

After updating from the old version of Clash to the new version, you will see the following error:

![](../../.gitbook/assets/378125d64dc2b271c9b1cafc42fdd634.png)

This is a known bug with the current version of clash. It's not related to the Wannaflix configuration API.&#x20;

To solve this, click the ClashX icon in the status bar and select "Configure" - "Open Configuration Folder".

Delete the config.yaml file in the open Finder window.

![](../../.gitbook/assets/f2156562aac93e23b2730837ecbbc05c.png)

Then exit and restart the ClashX application.
{% endtab %}
{% endtabs %}

##

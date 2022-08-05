# Clash For Windows

{% hint style="warning" %}
This guide is for Clash for Windows **version 0.13.6** and up.
{% endhint %}

{% hint style="warning" %}
Clash for Windows does NOT support the new VLESS+XTLS protocol. We recommend using [Netch ](netch-1.md)or [v2rayN ](v2rayn-recommended.md)instead.

Clash for Windows is not officially supported but we provide this guide for those that may want to use it.
{% endhint %}

Updated: August 13, 2020

Clash for Windows **version 0.13.6 and up** supports both v2ray AND ShadowsocksR. It also supports the TUN/TAP engine for capturing packets. This means it can run games without needing additional software.&#x20;

## Download and install Clash

[Click here](https://get.wannaflix.link/1bae24) to download the app. Once downloaded, double-click it to install.

{% hint style="info" %}
Version: v0.19.12

Released on: March 11, 2022
{% endhint %}

{% hint style="success" %}
Alternative mirrors:

Download on [Github](https://github.com/Fndroid/clash\_for\_windows\_pkg/releases)&#x20;
{% endhint %}

Once installed, you can find it on your desktop, or by doing a search for "Clash" in the windows search bar.

Double-click to start the app.

{% hint style="info" %}
You will find the app in the tray at the bottom right corner of the screen.

The app icon is a blue cat.
{% endhint %}

## Add the servers

### Copy the API

1. Login to your dashboard
2. Select "Clash for Windows" in the dropdown for Windows
3. Click "Copy API"

### Paste the API&#x20;

1. Open Clash by double-clicking on the app icon in the tray on the bottom right corner of your screen (blue cat icon)
2. Go to "Profile" (left-hand menu)
3. Paste the API in the "Download from URL" box and click "Download"

Your server list has now been downloaded to the app.

## Connect

### Select a server and mode

1. Go to "Proxies" (left-hand menu)
2. Select either Global mode or Proxy mode from the top (see box below)
3. Select a server from the list

{% hint style="info" %}
Modes:

Global - All websites go through WannaFlix

Rule - Websites go to different servers based on pre-configured rule sets.
{% endhint %}

### Connect

1. Go to the "General" tab
2. Toggle the "System Proxy" switch

You are now connected.

{% hint style="info" %}
To disconnect: Toggle the "System Proxy" switch again
{% endhint %}

{% hint style="danger" %}
Make sure to **turn the "System Proxy" switch OFF before quiting the app** or you won't have any internet if you do so (i.e. a kill-switch).

To fix it, restart the app and turn the "System Proxy" switch OFF and then quit the app.
{% endhint %}

## Additional Steps \[IMPORTANT]

### Install the TAP engine

If you want to play games with Clash or have all apps go through Clash, you need to install the TAP engine.

1. Go to the "General" tab
2. Click "Manage" next to "TAP Device"
3. Click "Install"

Now reconnect.&#x20;

### Windows Store apps

Windows Store apps do not go through the VPN by default, even when TAP is enabled. You need to force them by using the UWP Loopback Helper.

1. Go to the "General" tab
2. Click "Launch Helper" next to "UWP Loopback"
3. If there's a popup click "No"
4. Select all the apps you want to force through the VPN
5. Click "Save Changes"

### Enable Start with Windows

If you want Clash to automatically start when you boot your computer, you need to enable this option.

1. Go to the "General" tab
2. Toggle the "Start with Windows" switch

### Kill all connections when changing server

By default, old connections will not be redirected to the new server but will continue going to the old server until they timeout.

This creates problems when you're switching servers to watch Netflix or if you need a specific IP address as the websites you've just visited will still be going through the old server.

To kill all connections (and therefore forcibly reconnect via the new server), do this:

1. Go to "Settings"
2. Scroll down to "Connections"
3. Select "All" next to "Break when proxy change"
4. Also toggle "Break when Profile change" and "Break when Mode change"

## Troubleshooting

To be done.

### How can I play games with Clash for Windows?

You need to install the TAP Device (see [above](clash-for-windows-new.md#install-the-tap-engine)), and connect to a server that supports UDP.

### Spotify/OneDrive/Other app doesn't work

Windows Store apps don't go through Clash by default. You need to force them to go through by using the UWP Loopback Helper (see [above](clash-for-windows-new.md#windows-store-apps)).

If it still doesn't work, make sure you've installed the TAP interface (see above).

### Netflix/other website is using another server to connect instead of the one I selected.

You have probably selected "Rule" mode and the Netflix website is being redirected to another server based on the Netflix rule set. Select the server you want under "Netflix" in the server list.

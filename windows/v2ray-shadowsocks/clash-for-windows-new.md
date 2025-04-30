# Clash For Windows (Legacy app)

Updated: April 16, 2024

{% hint style="success" %}
**This app is the recommended app for Windows.**&#x20;

**However, if you would like a more simple interface, consider using** [**v2rayN**](v2rayn-recommended.md) **instead. Both work equally well.**&#x20;

**Clash supports split tunneling, whereas v2rayN sends all traffic through the same server. Split tunneling is more complicated to set up and can create issues if it is not set up correctly.**&#x20;
{% endhint %}

{% hint style="info" %}
This guide is for Clash for Windows **version 0.20.5** and up.
{% endhint %}

Clash for Windows **version 0.20.5 and up** supports both Trojan AND Shadowsocks. It also supports the TUN engine for capturing packets, and provides support for the Windows app store via UWP. This means it can run games without needing additional software.&#x20;

## STEP 1: Download and install Clash

[Click here](https://cdn-edge.wannaflix.net/Clash.for.Windows.Setup.0.20.39.exe) to download the app. Once downloaded, double-click it to install.

{% hint style="info" %}
Version: v0.20.39

Released on: October, 2023
{% endhint %}

{% hint style="success" %}
Alternative mirrors:

Download on [Github](https://github.com/Kuingsmile/clash-core/releases/tag/cfw)&#x20;
{% endhint %}

Once installed, you can find it on your desktop, or by doing a search for "Clash" in the windows search bar.

Double-click to start the app.

{% hint style="info" %}
You will find the app in the tray at the bottom right corner of the screen.

The app icon is a blue cat.
{% endhint %}

## STEP 2: Add the servers

### Copy the API

1. Login to your dashboard
2. Select "Clash for Windows" in the dropdown for Windows
3. Click "Copy API"

### Paste the API&#x20;

1. Open Clash by double-clicking on the app icon in the tray on the bottom right corner of your screen (blue cat icon)
2. Go to "Profile" (left-hand menu)
3. Paste the API in the "Download from a URL" box and click "Download"

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.36.13 PM.png" alt=""><figcaption></figcaption></figure>

Your server list has now been downloaded to the app.

{% hint style="success" %}
**IMPORTANT:**

Make sure you select the newly downloaded server config file, and not the default.
{% endhint %}

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.38.45 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
We **HIGHLY** recommend to set the API to auto-update the server list at least once a day (preferably every 12 hours).&#x20;

To do so, right click on the profile you just added, and go to settings. Under "Update Interval (hours)" type "12", then click OK.
{% endhint %}

<div data-full-width="false"><figure><img src="../../.gitbook/assets/Screenshot 2023-03-02 at 9.02.01 PM.png" alt="" width="306"><figcaption></figcaption></figure></div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-03-02 at 9.03.20 PM.png" alt="" width="375"><figcaption><p>Set the Update Interval to every 12 hours</p></figcaption></figure>

## STEP 3: Select a server

### OPTION 1: Simple Setup - all websites through 1 server

**If you are unfamiliar with Clash, we recommend this setup.**

1. Go to "Proxies" (left-hand menu)
2. Select Global mode from the top (see image below)
3. Select a server from the list

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 5.44.11 PM.png" alt=""><figcaption></figcaption></figure>



### OPTION 2: Split-tunneling Setup - decide which server each site will go through

1. Go to "Proxies" (left-hand menu)
2. Select Rule mode from the top (see box below)
3. Select a server from the list under "WannaFlix". This will be your main server.
4. You can also select a different server for services like Netflix and Youtube.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.40.24 PM.png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
Modes:

Global - All websites go through one WannaFlix server

Rule - Websites go to different servers based on pre-configured rule sets.
{% endhint %}

## STEP 4: Connect

1. Go to the "General" tab
2. Toggle the "System Proxy" switch

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.42.39 PM.png" alt=""><figcaption></figcaption></figure>

You are now connected.

{% hint style="info" %}
To disconnect: Toggle the "System Proxy" switch again
{% endhint %}

{% hint style="danger" %}
Make sure to **turn the "System Proxy" switch OFF before quiting the app** or you won't have any internet if you do so (i.e. it doubles as a kill-switch).

To fix it, restart the app and turn the "System Proxy" switch OFF and then quit the app.
{% endhint %}

## Additional Steps \[IMPORTANT READ]

### Install the TUN engine

If you want to play games with Clash or have all apps go through Clash, you need to install the TUN engine.

1. Go to the "General" tab
2. Click "Manage" next to "Service Mode"
3. Click "Install"
4. If you get any popups, click YES.

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.44.18 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.45.06 PM.png" alt=""><figcaption></figcaption></figure>

If it is correctly installed, the globe will turn green.&#x20;

Now disable System Proxy, and enable TUN mode.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.51.45 PM.png" alt=""><figcaption></figcaption></figure>

### Windows Store apps

Windows Store apps do not go through the VPN by default, even when TUN/TAP is enabled. You need to force them by using the UWP Loopback Helper.

1. Go to the "General" tab
2. Click "Launch Helper" next to "UWP Loopback"
3. If there's a popup click "YES"
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

To be done. Please submit any issues to the team. Common issues and how to fix them will be added here.

### How can I update the server list?

Go to profiles, and click on the refresh icon next to the profile you want to update.

<figure><img src="../../.gitbook/assets/Screenshot 2023-03-02 at 9.05.04 PM.png" alt=""><figcaption></figcaption></figure>

### How can I play games with Clash for Windows?

You need to install the TUN Device (see [above](clash-for-windows-new.md#install-the-tap-engine)), and connect to a server that supports UDP.

### Spotify/OneDrive/Other app doesn't work

Windows Store apps don't go through Clash by default. You need to force them to go through by using the UWP Loopback Helper (see [above](clash-for-windows-new.md#windows-store-apps)).

If it still doesn't work, make sure you've installed the TUN interface (see above).

### Netflix/other website is using another server to connect instead of the one I selected.

You have probably selected "Rule" mode and the Netflix website is being redirected to another server based on the Netflix rule set. Select the server you want under "Netflix" in the server list.

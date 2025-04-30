# 👍 Clash Verge (Recommended)

Updated: May 1, 2025

{% hint style="success" %}
**This app is the recommended app for Windows.**

**If you are running and old Windows 7 computer, please use Clash for Windows instead.**&#x20;
{% endhint %}

{% hint style="info" %}
This guide is for Clash Verge **version 2.2.3** and up (April 2025 release).&#x20;
{% endhint %}

Clash Verge **version 2.2.3 and up** supports all major protocols, and works with all our servers. It also supports the TUN engine for capturing packets, and provides support for the Windows app store via UWP. This means it can run games without needing additional software.&#x20;

## STEP 1: Download and install Clash Verge

{% hint style="info" %}
Version: v2.2.3
{% endhint %}

{% hint style="success" %}
[**Click here**](https://wannaflix-sz-edge.b-cdn.net/clash/windows/Clash.Verge_2.2.3_x64-setup.exe) **to download the app.**&#x20;

Alternative mirrors:

* Download on [Github](https://github.com/clash-verge-rev/clash-verge-rev/releases)&#x20;
{% endhint %}

#### Install the Application

1. Double-click the `.exe` file.
2. Windows may show a security warning. Click **"More info"** → **"Run anyway"**.
3. Follow the installer steps (next, install, finish).

{% hint style="info" %}
Make sure to choose "English" as the language when installing.
{% endhint %}

**Run Clash Verge**

* Open the app. If prompted by Windows Firewall, allow access.

Once installed, you can find it on your desktop, or by doing a search for "Clash" in the windows search bar.

Double-click to start the app.

{% hint style="info" %}
You will find the app in the tray at the bottom right corner of the screen.

The app icon is a cat in a purple circle.&#x20;

![](<../.gitbook/assets/Screenshot 2025-04-30 at 11.18.33 AM.png>)
{% endhint %}

## STEP 2: Import your config

### Copy the API

1. Login to your dashboard
2. Select "Clash Verge" in the dropdown for Windows
3. Click "Copy API"

{% hint style="success" %}
### Different API types:

* **Simple API**: One proxy group, easy to set up, suitable for basic use. _**Recommended for new users.**_
* **Split-tunneling API**: Supports multiple proxy groups and service-based routing for advanced control.
* **Subconverter API**: A technical tool for advanced users to convert and customize subscription configs across different formats (Clash, Surge, etc.). \[Only if you know what it is]
{% endhint %}

### Paste the API&#x20;

1. Open Clash by double-clicking on the app icon in the tray on the bottom right corner of your screen (purple cat icon)
2. Go to "Profiles" (left-hand menu)&#x20;
3. Paste the API in the "Profile URL" box and click "IMPORT"

<figure><img src="../.gitbook/assets/Screenshot 2025-04-30 at 11.35.43 AM.png" alt=""><figcaption></figcaption></figure>

Your server list has now been downloaded to the app.

## STEP 3: Select a server and connect

### OPTION 1: Simple API

{% hint style="success" %}
**REMINDER: If you are unfamiliar with Clash, we recommend this setup.**&#x20;

**If you see a different setup that the screenshots, check that you got the correct config API from our website**
{% endhint %}

1. Go to "Home" (left-hand menu)
2. Under "Current Node" select a server from the list (see image below)
3. Under "Network Settings" toggle on "System Proxy"

<figure><img src="../.gitbook/assets/Screenshot 2025-04-30 at 12.39.14 PM.png" alt=""><figcaption></figcaption></figure>

### OPTION 2: Split-tunneling API - decide which server each site will go through

1. Go to "Home" (left-hand menu)
2. Under "Current Node" select "Wannaflix" as the group
3. Then, select a server from the list (see image below)
4. Under "Network Settings" toggle on "System Proxy"

<figure><img src="../.gitbook/assets/Screenshot 2025-04-30 at 1.02.10 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
### What are modes?

Rule - **Recommended.** Choose this option if you are in China. Websites go to different servers based on pre-configured rule sets.&#x20;

Global - All websites go through one Wannaflix server. Can cause Chinese sites to malfunction. Only choose this option if you are **NOT** in China.&#x20;

Direct - **Don't enable**. (Disables the VPN).

NOTE: If you are using the SIMPLE API, Rule mode does split tunneling for Chinese and foreign sites automatically (Chinese sites connect directly, not through the VPN, and overseas sites go through the VPN).
{% endhint %}

{% hint style="success" %}
### Configure split tunneling (Optional)

1. Click the **“Proxies”** tab in the left sidebar
2. Under **Proxy Groups** :
   * You'll see a list of different groups(like `Wannaflix`,  `🍎 Apple`, or `📺 Netflix`)
3. Click on the **group** name (e.g., `📺 Netflix`)
4. Select the desired server from the list (e.g., 🇯🇵 Japan, 🇸🇬 Singapore, etc.)
5. &#x20;That service will now go through your selected server.&#x20;
{% endhint %}

### You are now connected.

{% hint style="info" %}
To disconnect: Toggle the "System Proxy" switch again
{% endhint %}

{% hint style="danger" %}
Make sure to **turn the "System Proxy" switch OFF before quiting the app** or you won't have any internet if you do so (i.e. it doubles as a kill-switch).

To fix it, restart the app and turn the "System Proxy" switch OFF and then quit the app.
{% endhint %}

## FYI \[IMPORTANT READ]

### If you want to play games with Clash or have all apps go through Clash, you need to use TUN Mode instead of System Proxy

1. Go to the "Home" tab
2. Under "Network Settings", disable "System Proxy"
3. Select "TUN Mode", and toggle on

{% hint style="success" %}
When TUN mode is enabled, there is no need to enable system proxy.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2025-04-30 at 1.21.38 PM.png" alt=""><figcaption></figcaption></figure>

### Windows Store apps

Windows Store apps do not go through the VPN by default, even when TUN is enabled. You need to force them by using the UWP Loopback Helper.

1. Go to the "Settings" tab
2. Click "Open UWP tool"
3. If there's a popup click "YES"
4. Select all the apps you want to force through the VPN
5. Click "Save Changes"

### Enable Start with Windows

If you want Clash to automatically start when you boot your computer, you need to enable this option.

1. Go to the "Settings" tab
2. Toggle the "Auto Launch" switch

### Kill all connections when changing server

By default, old connections will not be redirected to the new server but will continue going to the old server until they timeout.

This creates problems when you're switching servers to watch Netflix or if you need a specific IP address as the websites you've just visited will still be going through the old server.

To kill all connections (and therefore forcibly reconnect via the new server), do this:

1. Go to "Connections" tab
2. Click "CLOSE ALL"

## FAQ

### How can I update the server list?

Go to profiles, and click on the refresh icon next to the profile you want to update.

<figure><img src="../.gitbook/assets/Screenshot 2023-03-02 at 9.05.04 PM.png" alt=""><figcaption></figcaption></figure>

### How can I play games with Clash for Windows?

You need to install the TUN Device (see [above](v2ray-shadowsocks/clash-for-windows-new.md#install-the-tap-engine)), and connect to a server that supports UDP.

### Spotify/OneDrive/Other app doesn't work

Windows Store apps don't go through Clash by default. You need to force them to go through by using the UWP Loopback Helper (see [above](v2ray-shadowsocks/clash-for-windows-new.md#windows-store-apps)).

If it still doesn't work, make sure you've installed the TUN interface (see above).

### Netflix/other website is using another server to connect instead of the one I selected.

You have probably selected "Rule" mode and the Netflix website is being redirected to another server based on the Netflix rule set. Select the server you want under "Netflix" in the server list.


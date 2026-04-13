# 👍 FlClash (Recommended)

Updated: April 13, 2026

Time to complete tutorial: 5 minutes

## STEP 1: Download and install FlClash

{% hint style="success" %}
### Version: v0.8.92

### Download:

Apple Silicone (M-series Macs): [DOWNLOAD](https://cdn-edge.wannaflix.net/clash/macos/FlClash-0.8.92-macos-applesilicon.dmg)\
Intel chips: [DOWNLOAD](https://cdn-edge.wannaflix.net/clash/macos/FlClash-0.8.92-macos-amd64.dmg)

### Alternative mirrors:

Download on [Github](https://github.com/chen08209/FlClash/releases)
{% endhint %}

### Install the Application

1. Double-click the `.dmg` file.&#x20;
2. Drag the FlClash icon to the "applications" box

#### Allow FlClash to run on your Mac

If you encounter a warning stating that the app cannot be opened because **Apple cannot check it for malicious software**, follow these steps:

1. Click "DONE" on the warning box

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.19.48 PM.png" alt="" width="262"><figcaption></figcaption></figure>

2. Go to **System Settings > Privacy & Security**.
3. Click **"Open Anyway"** next to the warning about FlClash.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.27.19 PM.png" alt=""><figcaption></figcaption></figure>

4. Confirm by clicking **"Open"** in the subsequent dialog.
5. If you get an additional box requesting permission for  `osacript` , please enter your password and allow it to run

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.21.52 PM.png" alt="" width="262"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.30.43 PM.png" alt="" width="256"><figcaption></figcaption></figure>

{% hint style="info" %}
### Source

[https://support.apple.com/guide/mac-help/apple-cant-check-app-for-malicious-software-mchleab3a043/mac](https://support.apple.com/guide/mac-help/apple-cant-check-app-for-malicious-software-mchleab3a043/mac)
{% endhint %}

### **Launch FlClash**

1. Find `FlClash` in your applications and double-click on it to launch it
2. You should see it in your dock

<div align="left"><figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.54.51 PM.png" alt=""><figcaption></figcaption></figure></div>

## STEP 2: Import your config

### Copy the API

1. Login to your [client area](https://wannaflix.com/clientarea.php) dashboard
2. Select "FlClash" in the dropdown for MacOS
3. Click "Copy API"

{% hint style="success" %}
### Different API types:

* **Simple API**: One proxy group, easy to set up, suitable for basic use. _**Recommended for new users.**_
* **Split-tunneling API**: Supports multiple proxy groups and service-based routing for advanced control.
{% endhint %}

### Paste the API&#x20;

1. Open **FlClash**
2. Go to the **folder icon**
3. Click **"Add profile"**

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.34.42 PM.png" alt=""><figcaption></figcaption></figure>

4. Select the **URL** option

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.35.41 PM.png" alt="" width="353"><figcaption></figcaption></figure>

5. Paste your API in the box and click **Submit**

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.36.29 PM.png" alt="" width="350"><figcaption></figcaption></figure>

Your config file will be downloaded.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.59.05 PM.png" alt="" width="375"><figcaption></figcaption></figure>

## STEP 3: Select a server and connect

1. Click on the `Proxies` icon (2nd menu item from the top)
2. Click `Delay Test` to test which servers can be connected to
3. Select a server with a number next to it

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.45.44 PM.png" alt=""><figcaption></figcaption></figure>

4. Go to the Dashboard (first icon from the top)
5. Make sure `System proxy` is enabled
6. Click the **`Start`** button to connect

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.51.42 PM.png" alt=""><figcaption></figcaption></figure>

### You are now connected.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 5.53.51 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
### How to disconnect

Click the Pause button
{% endhint %}

## \[IMPORTANT READ]

### If you want to play games with Clash or have all apps go through Clash, you need to use TUN Mode instead of System Proxy

1. Enable **TUN**

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 6.07.17 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
When TUN mode is enabled, there is no need to enable system proxy. You can toggle off `System proxy`
{% endhint %}

## FAQ

### How can I update the server list?

Go to **Profiles** and click the **refresh** button

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 6.09.37 PM.png" alt=""><figcaption></figcaption></figure>

### How can I play games with ClashX?

You need to use Tun Mode (see above).

### Netflix/other website is using another server to connect instead of the one I selected.

You are probably using the **SPLIT TUNNELING API** and the Netflix website is being redirected to another server based on the Netflix rule set. Select the server you want under the "Netflix" tab in the server list.

<figure><img src="../.gitbook/assets/Screenshot 2026-04-13 at 6.11.50 PM.png" alt=""><figcaption></figcaption></figure>

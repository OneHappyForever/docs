# V2rayN

{% hint style="success" %}
**V2rayN is stable and the UI is quite good. However, it does not support gaming or Windows Store apps, and only supports System Proxy mode. If you need these features, please consider switching to** [**Clash for Windows**](../../installation-guides/windows/clash-for-windows.md)**.**
{% endhint %}

Updated: April 16, 2024

Recommended environment:  Windows 10+

## Version 6.42 and up (April 16, 2024)

{% hint style="success" %}
We HIGHLY recommend upgrading to version 6 or above.
{% endhint %}

### STEP 1: Download and install V2rayN

[Click here](https://cdn-edge.wannaflix.net/v2rayN-With-Core-6.42.zip) to download the app. It will download it in .ZIP format.

{% hint style="success" %}
Alternative mirrors:

Download on [Github](https://github.com/2dust/v2rayN/releases) (it will download as V2rayN-Core.zip instead of V2rayN.zip; look for that filename instead in the next step)
{% endhint %}

{% hint style="danger" %}
If you want the **previous** 5.36 version (if you have an older version of Windows) you can [download it here](https://cdn-edge.wannaflix.net/v2rayN-Core-5.36.zip).
{% endhint %}

Find the V2rayN-With-Core.zip file in your download folder. Unzip it (right click > Extract all... ). Then, open the unzipped folder.&#x20;

Double-click on the "V2rayN" file to install.

{% hint style="warning" %}
Required dependencies:

**.NET framework version 8** or above from Microsoft. Older versions of Windows may not have the latest version of .NET.

Normally a popup will redirect you to the microsoft website upon install. You can also [**click here**](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-8.0.4-windows-x64-installer) to be redirected to Microsoft's website to download the .NET framework installer.
{% endhint %}

![](<../../.gitbook/assets/Screenshot 2024-04-16 at 6.56.32 PM.png>)

If there's a pop-up, click "run".

{% hint style="info" %}
Once installed, you can find the app by searching for "v2rayN" in the search box next to the start menu.&#x20;

You can then find V2rayN in the tray at the bottom right corner of your screen.
{% endhint %}

{% hint style="danger" %}
If you downloaded the file from github, it will default to Chinese. Scroll down to the troubleshooting section to find out how to change the language.
{% endhint %}

### STEP 2: Add the servers

#### Get the api link

1. Go to your [client area](https://wannaflix.com/clientarea.php)&#x20;
2. Under "Windows", select "V2rayN (v6.42+)"
3. Click on the "Copy API" button to copy the API

{% hint style="info" %}
The API link should start with https://api.wannaflix.com/**apiv3.php**?type=**v2rayn**
{% endhint %}

#### Paste the api link into the app

1. Open the app by double clicking on the v2rayN icon (blue V) in the tray on the bottom right corner of your screen.

![](../../.gitbook/assets/tempsnip.png)

2\. Go to "Subscription group" > "Subscription group settings"

![](<../../.gitbook/assets/Screenshot 2024-04-16 at 6.59.19 PM.png>)

3\. Click "Add"&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 7.00.06 PM.png" alt=""><figcaption></figcaption></figure>

4\. Type "WannaFlix" in the Remarks box; Paste the API into the URL box; and set the Nabled Update to 1500. Then click Confirm.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 7.01.04 PM.png" alt=""><figcaption></figcaption></figure>

6\. Go to "Subscription group" > "Update subscription without proxy"

![](<../../.gitbook/assets/Screenshot 2024-04-16 at 7.03.25 PM.png>)

### STEP 3: Select a server

Double-click on a server to select it (it will turn blue)

![](<../../.gitbook/assets/Screenshot 2024-04-16 at 7.07.07 PM.png>)

### STEP 4: Start the VPN

At the bottom, change the system proxy dropdown to "Set system proxy"

{% hint style="success" %}
To turn the VPN off, switch it back to "Clear system proxy"
{% endhint %}

![](<../../.gitbook/assets/Screenshot 2024-04-16 at 7.05.10 PM.png>)

***

## Troubleshooting

### The app is in Chinese! How to switch the language to English?

1. Tap the 3 dots icon, and change the last drop-down to "en"

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 6.37.09 PM.png" alt=""><figcaption></figcaption></figure>

2. Then restart the app. Find the icon in the tray, right click on it, and tap on the "推出" button

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 6.57.33 PM.png" alt="" width="375"><figcaption></figcaption></figure>

### Some apps don't work with V2rayN

In this case, try using TUN mode. Switch it on at the bottom of the app.&#x20;

TUN will need to be installed the first time you run it. If there is a popup, allow the installation.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 7.20.47 PM.png" alt=""><figcaption></figcaption></figure>

### Window Store apps don't work!

Windows sometimes disregards the VPN for its own app store. You need to set up the UWP helper tool to make it work.

In the new window, select the apps you want to force Windows to run through the VPN. You can click "Exempt all" to force all Windows apps to go through WannaFlix. Don't forget to "Save Changes" too.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 7.23.53 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 7.25.11 PM.png" alt=""><figcaption></figcaption></figure>

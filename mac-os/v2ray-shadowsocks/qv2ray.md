# Qv2ray \(NEW PROTOCOL\)

Updated: March 17, 2021

{% hint style="warning" %}
**IMPORTANT:**

We do not officially support Qv2ray. This app doesn't not always install successfully and may have permissions issues on some Macs. Should a permission issue occur, we do not have a fix at this time. 

However, you are welcome to try. It may well work for you. We just don't want to make any promises.
{% endhint %}

Qv2ray is the only app that supports the latest v2ray protocol on Mac \(other than Shadowrocket for M1 Macs\).

It is a little complicated to setup as you need to download the graphical user interface separately from the core app. 

We have tried to make this guide as simple and straightforward as possible so you can get it up and running easily.

So here goes!

## Download and Install

[Click here](https://wannaflix.com/dl.php?type=d&id=33) to download the graphical user interface \(GUI\) app.

Install the app.

{% hint style="info" %}
IMPORTANT: You need the pre-release version for it to work with our latest API.

If you are downloading from github, download the latest pre-release \(right now it's at[ version 2.7.0-pre2](https://github.com/Qv2ray/Qv2ray/releases/download/v2.7.0-pre2/Qv2ray.v2.7.0-pre2.macOS-x64.dmg)\)
{% endhint %}

Now we need to install Xray-core:

Open terminal and run the following commands.

Step 1: Add tap

```text
brew tap N4FA/xray
```

Step 2: Install Xray-core

```text
brew install xray-core
```

{% hint style="danger" %}
Qv2ray does NOT contain the necessary files to run v2ray. You **MUST** install Xray-core for it to work.
{% endhint %}

{% hint style="info" %}
If you don't have homebrew installed or get the error "command not found", you need to install homebrew:

Copy-paste the following in your terminal:

xcode-select --install

/bin/bash -c "$\(curl -fsSL [https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)\)"

If you encounter a permission issue while installing brew, paste the following into your terminal:

sudo chgrp -R admin $\(brew --prefix\)/ __

sudo chmod -R g+w $\(brew --prefix\)/
{% endhint %}

Now run the Qv2ray GUI you downloaded before.

Go to Qv2ray &gt; Preferences &gt; Kernel Settings:

Replace the v2ray executable path to: /usr/local/Cellar/xray-core/{XRAY VERSION}/bin/xray

Replace the old v2ray assets path to: /usr/local/Cellar/xray-core/{XRAY VERSION}/share/xray-core

{% hint style="danger" %}
**IMPORTANT**: the {XRAY VERSION} part **MUST** be replaced with the current Xray-core version that you downloaded. 

The current version at the time this was written is 1.4.0 but  it will likely be higher by the time you install it on your Mac.

To find out your version, open your file explorer and navigate to this folder: /usr/local/Cellar/xray-core

You'll find the version in the name of the folder there.
{% endhint %}

## Add your servers

### Get the API link

1. Go to your [client area](https://wannaflix.com/clientarea.php) dashboard
2. Under the Mac OS &gt; Qv2ray, click "COPY API" to copy the API

### Paste the API

1. Open your Qv2ray app
2. Go to Qv2ray &gt; Groups &gt; Subscription Settings
3. Paste the API into "Subscription Address" and click "Update subscription"
4. Click OK

## Connect

Double-click on a server to connect.

Or, select a server and click on the "Play" button to the right to connect.

## Troubleshooting

We haven't received any reports of any issues with this app yet. If you encounter an issue, please reach out to us. If the issue affects multiple users, we'll add it here.


# Qv2ray

{% hint style="info" %}
Guide taken from the official documentation at [https://qv2ray.net/en/getting-started/](https://qv2ray.net/en/getting-started/)
{% endhint %}

## Download and Install

You can install Qv2ray via several methods:

### Method 1: Via an App Store

#### Snapcraft <a id="snapcraft"></a>

Follow the instructions on our [Snapcraft page](https://snapcraft.io/qv2ray).

```text
# To install the package:
$ snap install qv2ray
# snap install qv2ray --edge (dev branch)
# To update the package:
$ snap refresh qv2ray
```

#### Flathub <a id="flathub"></a>

1. Set up Flatpak environment according to the [official documentation](https://flatpak.org/setup/).
2. Install Qv2ray:

   ```text
   # To install the package:
   $ flatpak install com.github.Qv2ray
   # To update the package:
   $ flatpak update
   ```

### Method 2: Via AppImage 

Go to the[ official release page](https://github.com/Qv2ray/Qv2ray/releases) and download the Qv2ray.VERSION.linux-x64.AppImage version.

{% hint style="info" %}
 For Ubuntu 19.04 / Debian 10 \(or greater\): `qv2ray_VERSION_amd64.deb` \(Moved to [Qv2ray Debian Repository](https://qv2ray.github.io/debian/) since v2.6.1\)
{% endhint %}

{% hint style="info" %}
Notes for Linux AppImage users

Although we have bundled `glibc` and some basic C++ libraries into the **AppImage** package to support some old but supported distros, moving yourself to a newer version of Distro/OS is strongly recommended.
{% endhint %}

## Configuring V2ray Core

### Download the V2ray Core

 Go to [the official GitHub Release page of v2fly/v2ray-core](https://github.com/v2fly/v2ray-core/releases) and check the recent stable builds. Choose according to your platform in the asset files. 

For example, Windows 64-bit users may download `v2ray-windows-64.zip`, Mac OS users may download `v2ray-macos-64.zip`, and for most of the Linux users, `v2ray-linux-64.zip`.

### Place Your V2Ray Core <a id="place-your-v2ray-core"></a>

Extract the v2ray core files into a fixed position. As a default, it is suggested to extract the files into `$QV2RAY_CONFIG_PATH/vcore`, where `$QV2RAY_CONFIG_PATH` is the directory where Qv2ray store it’s data.

The directory `vcore` could be in one of these locations:

* `./config/` \(`config` subdirectory aside Qv2ray executable, which is recommended for Windows Users\)
* `~/.qv2ray/` \(in a dedicated directory of your home folder\)
* `~/.config/qv2ray/` \(standard XDG configuration path\)

Afterwards, please make sure that these files exists directly in your `vcore` directory:

1. `v2ray` / `v2ray`: core executable file
2. `v2ctl` / `v2ctl`: core controlling program
3. `geoip.dat`: IP rules database
4. `geosite.dat`: domain rules database

{% hint style="warning" %}
Special Hint for Linux / macOS Users

You should always grant **executable permission** to `v2ray` and `v2ctl`. This is usually done by executing `chmod +x` on these files.
{% endhint %}

### Configure Qv2ray to Use the Core <a id="configure-qv2ray-to-use-the-core"></a>

Open Qv2ray and go to Preference Window. In [**Core Settings**](qv2ray://open/preference/kernel), configure the following options:

* **Core Executable Path**: Set this to where your V2Ray executable exists. This can be the full path of your `v2ray.exe` on Windows, or that `v2ray` executable file on Linux / macOS.
* **V2Ray Assets Directory**: Set this to where `geoip.dat` and `geosite.dat` are located.

After configuring, you can click on **Check V2Ray Core Settings** button to validate your V2Ray core settings. Repeat trying until you get the check passed.

{% hint style="danger" %}
Never ever point **Core Executable Path** to **Qv2ray Executable**! This will not cause a fork bomb since Qv2ray is single-instanced. Do note that V2Ray Core Executable is like `v2ray` or `v2ray.exe`, instead of `qv2ray` or `qv2ray.exe`!
{% endhint %}

{% hint style="info" %}
Hint for Arch Linux Users

If you use `v2ray` package, the suggested configuration is as follows:

* **Core Executable Path**: `/usr/bin/v2ray`
* **V2Ray Assets Directory**: `/usr/share/v2ray`
{% endhint %}

## Add your servers

#### Get the api link

1. Go to your [client area](https://wannaflix.com/clientarea.php) dashboard
2. Click on the "Windows V2rayN" button in the API box to copy the API for Qv2ray \(it's the same format; we will be adding a specific api for Qv2ray soon\).

{% hint style="info" %}
The API link should start with https://api.wannaflix.link/apiv2.php?type=**v2rayn**
{% endhint %}

To import an API, follow these steps:

1. Click **Subscriptions** button in the main window.
2. In the [**SubscribeEditor**](qv2ray://open/group/connection) dialog, click the **Add subscription** icon button at the left-bottom corner.
3. Click to select the newly generated item in **Subscription List**.
4. Input your subscription information on the right side.
   * **Subscription Name**: Fill this as you wish.
   * **Subscription Address**: Use your API link mentioned above.
   * **Update Interval**: Change this according to your own demands.
5. Click **Update Subscription Data** button to update the server list and wait until the process finishes.
6. Click **OK** to apply the settings and close the dialog.

{% hint style="info" %}
Update through System Proxy

If you encounter connectivity problem with your API upstream \(eg: DNS Record Pollution, IP Address Blocking, etc.\), you may try to run with **Update Subscription with System Proxy** option on. However, it's better to inform the upstream as soon as possible, to fix the issue permanently.
{% endhint %}

## Configuring Softwares to Use Qv2ray <a id="step-4-configuring-softwares-to-use-qv2ray"></a>

Congratulations! There's only one step left in order to access the unlocked Internet!

### General Methods <a id="general-methods"></a>

#### Using System Proxy <a id="using-system-proxy"></a>

For **Windows** and **macOS** users, almost all of the applications will follow the system proxy settings. For **Linux** users, some applications such as Firefox and Chromium, but not all, will read and obey the proxy configurations in GNOME/KDE Settings.

Currently, automatic setting of system proxy is supported by Qv2ray, including **Windows**, **macOS** and **Linux** \(GNOME/KDE\). You may find System Proxy options of Qv2ray in the following positions:

* **Qv2ray Tray Menu**.
  1. Right click on the tray icon.
  2. In the popup menu, choose **System Proxy** -&gt; **Enable/Disable System Proxy**.
* **Qv2ray Preference Window**.
  1. Click **Preferences** button in the main window.
  2. In **Preference Window**, choose the tab [**Inbound Settings**](qv2ray://open/preference/inbound).
  3. Check the option **Set System Proxy**.
  4. Click **OK** to apply the settings.

{% hint style="info" %}
Linux Users: KDE/GNOME Proxy Settings

If you are using GNOME as your main desktop environment, you may find it quite useful to set a system proxy. That's because GNOME Proxy Settings is almost universally acknowledged.

However, KDE users may have a difficult time, since KDE Proxy Settings is more like a toy. Even KDE Applications themselves won't read and obey that configuration. In that case, you may seek for an alternative solution to configure your applications.
{% endhint %}

{% hint style="warning" %}
Windows Users: UWP Loopback Problem

By default, UWP applications are prohibited from using a proxy with a loopback address \(127.0.0.1\), so the system proxy settings will probably cause your UWP applications cease to work normally.

You can use some third-party tool to **enable UWP loopback** for your program to be proxied. We here present you [this program](https://qv2ray.net/EnableLoopback.zip) from [Fiddler](https://www.telerik.com/fiddler) project.
{% endhint %}

#### Configure Manually in Applications

**Telegram**

You can configure Telegram to use proxies in the app. Go to **Settings** -&gt; **Advanced** -&gt; **Network and proxy** and click **Connection type**, where **Proxy Settings** dialog will be opened.

In **Proxy Settings**, click **Add Proxy** button on the bottom. Choose SOCKS5/HTTP according to your own flavor and fill in the blanks with the information from Qv2ray Inbound Settings.

Finally, click on the proxy entry that you've just configured. You are done.

**Web Browsers**

Almost all web browsers support manual configuration of proxies. Taking Firefox as example, you can find this settings in **Preferences -&gt; General -&gt; Network -&gt; Manual Proxy Configuration**. Fill these fields with the information from Qv2ray Inbound Settings to use Qv2ray.

Using Proxy Plugins

To avoid switching back and forth among proxy configurations, you may want to use a third-party plugin \(eg: SwitchyOmega\) to enhance your browser. These plugins can help to implement a more sophisticated configuration, including multiple profiles and further traffic diversion.

**Java Applications**

For Java applications, you may use configure proxies through JVM arguments.

Here are some examples:

* Using SOCKS5:

  ```text
  java -DsocksProxyHost=127.0.0.1 -DsocksProxyPort=1088 -jar some-application.jar
  ```

* Using HTTP\(S\):

  ```text
  java -Dhttp.proxyHost=127.0.0.1 -Dhttp.proxyPort=8000 -Dhttps.proxyHost=127.0.0.1 -Dhttps.proxyPort=8000 -jar some-application.jar
  ```

Buggy Minecraft

Newer versions of Minecraft \(`>=1.5.2`\) won't follow JVM proxy settings. That is not Qv2ray's problem. If you really want to play Minecraft through proxy, consider setting up a Dokodemo-door inbound for that server and connect directly to `localhost`.

### Platform-dependent Methods <a id="platform-dependent-methods"></a>

#### Using Environment Variables <a id="using-environment-variables"></a>

Many CLI programs \(for example `curl` and `wget`\) will use the proxies given by `<PROTOCOL>_PROXY` environment variable.

Here is a configuration example:

```text
# Change the host and port according to Qv2ray inbound configuration
export HTTP_PROXY="http://127.0.0.1:8000"
export HTTPS_PROXY="http://127.0.0.1:8000"
```

If authentication is enabled in Qv2ray, use the following settings:

```text
# Change user/pass according to your configuration
export HTTP_PROXY="http://user:pass@127.0.0.1:8000"
export HTTPS_PROXY="http://user:pass@127.0.0.1:8000"
```

Note that if there is a special character in your username or password, you need to encode it. Here's a quick reference:

| `!` | `#` | `$` | `&` | `'` | `(` | `)` | `*` | `+` | `,` | `/` | `:` | `;` | `=` | `?` | `@` | `[` | `]` |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `%21` | `%23` | `%24` | `%26` | `%27` | `%28` | `%29` | `%2A` | `%2B` | `%2C` | `%2F` | `%3A` | `%3B` | `%3D` | `%3F` | `%40` | `%5B` | `%5D` |

Or enter the text you want to encode: 

For programs running in `sudo`, it is required to configure `sudo` to preserve these variables if you do not run `sudo` in a shell. Call `visudo` with root and add the following line:

```text
Defaults env_keep += "HTTP_PROXY HTTPS_PROXY"
```

Still, there are some programs who are using their own variables. For example, `rsync` uses `RSYNC_PROXY` for HTTP proxies:

```text
export RSYNC_PROXY=user:pass@127.0.0.1:8000
```

It is strongly recommended to read the manual of programs that you want to configure proxy with.

#### Using `proxychains` <a id="using-proxychains"></a>

If none of the above methods works, you can try using `proxychains`, which hijacks program's function/library to redirect network connections into your proxies.

First, you should install `proxychains-ng`. Installation methods varies with each operating system.

* [Linux/macOS](https://github.com/rofl0r/proxychains-ng)
* [Windows](https://github.com/shunf4/proxychains-windows)

Edit `/etc/proxychains.conf` \(for global proxychains\) or `$HOME/.proxychains/proxychains.conf` \(for user\), edit `[ProxyList]` section and change the proxy to SOCKS5 Proxy in Qv2ray:

```text
[ProxyList]
socks5  127.0.0.1  1088
```

After configuring `proxychains`, you may use `proxychains <program>` in terminal to make `proxychains` hijack the program to use the given proxy. If you are fed up with the noisy output, you may append `-q` option after `proxychains`.

One thing to note is that `proxychains` does not work with statically-linked programs, for example, Golang programs.


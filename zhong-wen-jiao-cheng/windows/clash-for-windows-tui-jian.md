# Clash for Windows (推荐）

指南更新日期：2024年4月16日

{% hint style="success" %}
本应用是Windows系统推荐使用的应用。 但是，如果您想要一个更简单的界面，可以考虑使用v2rayN。两者都同样有效。 Clash支持分流，而v2rayN则通过同一服务器发送所有流量。分流设置更复杂，如果设置不正确可能会导致问题。
{% endhint %}

{% hint style="info" %}
本指南适用于Clash for Windows 0.20.5版本及以上。
{% endhint %}

Clash for Windows 0.20.5版本及以上同时支持Trojan和Shadowsocks协议。它还支持用于捕获数据包的TUN引擎，并通过UWP提供对Windows应用商店的支持。这意味着它可以运行游戏而无需额外软件。

## 步骤1：下载并安装Clash

[点击此处](https://cdn-edge.wannaflix.net/Clash.for.Windows.Setup.0.20.39.exe)下载应用。下载后，双击安装。

{% hint style="info" %}
版本：v0.20.39&#x20;

发布日期：2023年10月
{% endhint %}

{% hint style="success" %}
替代下载镜像：

[Github](https://github.com/Kuingsmile/clash-core/releases/tag/cfw)  上下载
{% endhint %}

安装完成后，您可以在桌面上找到它，或在Windows搜索栏中搜索"Clash"。

双击启动应用。

{% hint style="info" %}
您可以在屏幕右下角的托盘中找到该应用。

应用图标是一只蓝色的猫。
{% endhint %}

## 步骤2：添加服务器

### 复制API

1. 登录您的仪表板
2. 在Windows下拉菜单中选择"Clash for Windows"
3. 点击"复制API"

### 粘贴API

1. 通过双击屏幕右下角托盘中的应用图标（蓝色猫图标）打开Clash
2. 转到"配置文件"（左侧菜单）
3. 将API粘贴到"从URL下载"框中，然后点击"下载"

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.36.13 PM.png" alt=""><figcaption></figcaption></figure>

您的服务器列表现已下载到应用中。

{% hint style="success" %}
**重要提示：**&#x20;

确保选择新下载的服务器配置文件，而不是默认配置文件。
{% endhint %}

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.38.45 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
我们强烈建议将API设置为每天至少自动更新一次服务器列表（最好每12小时一次）。&#x20;

要执行此操作，请右键单击刚刚添加的配置文件，然后转到设置。在"更新间隔（小时）"下输入"12"，然后点击确定。
{% endhint %}

<div data-full-width="false">

<figure><img src="../../.gitbook/assets/Screenshot 2023-03-02 at 9.02.01 PM.png" alt="" width="306"><figcaption></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-03-02 at 9.03.20 PM.png" alt="" width="375"><figcaption><p>Set the Update Interval to every 12 hours</p></figcaption></figure>

## 步骤3：选择服务器

### 选项1：简单设置 - 所有网站通过1个服务器&#x20;

如果您不熟悉Clash，我们推荐此设置。

1. 转到"代理"（左侧菜单）
2. 从顶部选择全局模式（参见下图）
3. 从列表中选择一个服务器

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-16 at 5.44.11 PM.png" alt=""><figcaption></figcaption></figure>



### 选项2：分流设置 - 决定每个网站通过哪个服务器

1. 转到"代理"（左侧菜单）
2. 从顶部选择规则模式（参见下面的框）
3. 在"WannaFlix"下从列表中选择一个服务器。这将是您的主要服务器。
4. 您还可以为Netflix和YouTube等服务选择不同的服务器。

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.40.24 PM.png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
模式：&#x20;

全局 - 所有网站通过一个WannaFlix服务器&#x20;

规则 - 网站根据预配置的规则集转到不同的服务器
{% endhint %}

### 步骤4：连接

1. 转到"常规"标签页
2. 切换"系统代理"开关

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.42.39 PM.png" alt=""><figcaption></figcaption></figure>

您现在已连接。

{% hint style="info" %}
断开连接：再次切换"系统代理"开关
{% endhint %}

{% hint style="danger" %}
请确保在退出应用之前关闭"系统代理"开关，否则您将无法上网（即它也可以作为一个终止开关）。&#x20;

要修复此问题，请重新启动应用并关闭"系统代理"开关，然后退出应用。
{% endhint %}

## 其他步骤 \[重要阅读]

### 安装TUN引擎&#x20;

如果您想用Clash玩游戏或让所有应用通过Clash，您需要安装TUN引擎。

1. 转到"常规"标签页
2. 点击"服务模式"旁边的"管理"
3. 点击"安装"
4. 如果出现任何弹窗，请点击"是"。

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.44.18 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.45.06 PM.png" alt=""><figcaption></figcaption></figure>

如果正确安装，地球图标将变为绿色。&#x20;

现在禁用系统代理，并启用TUN模式。

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-28 at 5.51.45 PM.png" alt=""><figcaption></figcaption></figure>

### Windows商店应用&#x20;

默认情况下，Windows商店应用不会通过VPN，即使启用了TUN/TAP。您需要使用UWP Loopback Helper强制它们通过。

1. 转到"常规"标签页
2. 点击"UWP环回"旁边的"启动助手"
3. 如果出现弹窗，请点击"是"
4. 选择您想强制通过VPN的所有应用
5. 点击"保存更改"

### 随Windows启动&#x20;

如果您希望Clash在计算机启动时自动启动，您需要启用此选项。

1. 转到"常规"标签页
2. 切换"随Windows启动"开关

### 更换服务器时终止所有连接

&#x20;默认情况下，旧连接不会重定向到新服务器，而是会继续通过旧服务器直到超时。 当您切换服务器以观看Netflix或需要特定IP地址时，这会造成问题，因为您刚刚访问的网站仍将通过旧服务器。

要终止所有连接（从而强制通过新服务器重新连接），请执行以下操作：

1. 转到"设置"
2. 滚动到"连接"
3. 在"代理变更时断开"旁边选择"全部"
4. 同时切换"配置变更时断开"和"模式变更时断开"

### 故障排除

待完成。请将任何问题提交给团队。常见问题及其解决方法将添加在此处。

### **如何更新服务器列表？**&#x20;

转到配置文件，点击您想更新的配置文件旁边的刷新图标。

<figure><img src="../../.gitbook/assets/Screenshot 2023-03-02 at 9.05.04 PM.png" alt=""><figcaption></figcaption></figure>

### 如何使用Clash for Windows玩游戏？&#x20;

您需要安装TUN设备（见上文），并连接到支持UDP的服务器。

### Spotify/OneDrive/其他应用不工作&#x20;

Windows商店应用默认不通过Clash。您需要使用UWP Loopback Helper强制它们通过（见上文）。&#x20;

如果仍然不工作，请确保您已安装TUN接口（见上文）。

### Netflix/其他网站使用另一个服务器连接，而不是我选择的那个。&#x20;

您可能选择了"规则"模式，Netflix网站根据Netflix规则集被重定向到另一个服务器。在服务器列表中的"Netflix"下选择您想要的服务器。

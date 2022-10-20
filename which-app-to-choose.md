# Which App to Choose?

Updated: August 13, 2021

{% hint style="info" %}
**GLOSSARY**

_Officially supported:_ Apps we recommend. We provide installation and troubleshooting support on these apps only. Other apps are only on a best-effort basis.

_Stability:_ A measurement of the frequency of disconnections and speed fluctuations, as well as the  likelihood of encountering various issues.
{% endhint %}

## Windows

Recommendation: Netch or V2rayN for Xray. Netch or Clash for Shadowsocks. Netch for gaming. If you are still running v2ray, please update to Xray as soon as possible (you will need to get the latest app versions from our website and the new API for it).

{% hint style="info" %}
If you don't need to game with it, we personally find v2rayN easier to use.&#x20;

Both Netch and V2rayN run on the same Xray-core, so both will give you about the same speeds.

Clash... is always behind the curve when it comes to protocol support. But some prefer the UI and the ability to add their own split-tunneling rules.
{% endhint %}

|                      |                   v2rayN                   | Netch |                     SSR                    | Clash | OpenVPN |
| -------------------- | :----------------------------------------: | :---: | :----------------------------------------: | :---: | :-----: |
| Officially supported |                      ✅                     |   ✅   |                      ✅                     |   ❌   |    ✅    |
| Trojan               |                      ✅                     |   ✅   |                      ❌                     |   ✅   |    ❌    |
| Xray                 |                      ✅                     |   ✅   |                      ❌                     |   ❌   |    ❌    |
| v2ray                |                      ✅                     |   ✅   |                      ❌                     |   ✅   |    ❌    |
| SSR                  |                      ❌                     |   ✅   |                      ✅                     |   ✅   |    ❌    |
| Eclipse              |                      ❌                     |   ❌   |                      ❌                     |   ❌   |    ✅    |
| Ease of Use          |                      ✅                     |   ✅   |                     🟧                     |   🟨  |    🟨   |
| Speed                |                      ✅                     |   ✅   |                      ✅                     |   ✅   |    🟧   |
| Stability            |                      ✅                     |   🟨  |                      ✅                     |   ✅   |    🟨   |
| TCP                  |                      ✅                     |   ✅   |                      ✅                     |   ✅   |    ✅    |
| UDP                  |                     🟨                     |   ✅   |                      ✅                     |   ✅   |    ✅    |
| Netflix support      |                      ✅                     |   ✅   |                      ✅                     |   ✅   |    🟧   |
| Gaming               | <p>🟧</p><p>May need separate software</p> |   ✅   | <p>🟨</p><p>May need separate software</p> |   ✅   |    🟥   |

## Mac OS

Recommendation: Shadowrocket if you have an M1 Mac. ClashX otherwise. Please note that ClashX does not support the new VLESS+XTLS protocol, only the older VMESS protocol.

If you need SSR servers, then download the latest ClashX version (at the very least, version 1.30.1 and up).&#x20;

{% hint style="warning" %}
ONLY use Qv2ray if you are up to the challenge. It is not an easy app to setup, even if it is the only app that supports Xray.
{% endhint %}

|                      | Shadowrocket (M1) |                             ClashX                             |                              V2rayU                             | Tunnelblick |
| -------------------- | :---------------: | :------------------------------------------------------------: | :-------------------------------------------------------------: | :---------: |
| Officially supported |         ✅         |                                ✅                               |                                ❌                                |      ✅      |
| Trojan               |         ✅         |                                ✅                               |                                ❌                                |      ❌      |
| Xray                 |         ✅         |                                ❌                               |                                ✅                                |      ❌      |
| v2ray                |         ✅         |                                ✅                               |                                ✅                                |      ❌      |
| SSR                  |         ✅         |                                ✅                               |                                ❌                                |      ❌      |
| Eclipse              |         ❌         |                                ❌                               |                                ❌                                |      ✅      |
| Ease of Use          |         ✅         |                                ✅                               |                                ✅                                |      🟨     |
| Speed                |         ✅         |                                ✅                               |                                ✅                                |      🟧     |
| Stability            |         ✅         |                                ✅                               |                                ✅                                |      🟨     |
| TCP                  |         ✅         |                                ✅                               |                                ✅                                |      ✅      |
| UDP                  |         ✅         |                                ✅                               |                                ✅                                |      ✅      |
| Netflix support      |         ✅         |                                ✅                               |                                ✅                                |      🟧     |
| Gaming               |         ✅         | <p>✅</p><p>May </p><p>need </p><p>separate </p><p>software</p> | <p>🟨</p><p>May </p><p>need </p><p>separate </p><p>software</p> |      🟥     |

## iOS

Recommendation: Shadowrocket. Only Shadowrocket.

|                      | Shadowrocket | Quantumult | OpenVPN |
| -------------------- | :----------: | :--------: | :-----: |
| Officially supported |       ✅      |      ❌     |    ✅    |
| Trojan               |       ✅      |      ❌     |    ❌    |
| Xray                 |       ✅      |      ❌     |    ❌    |
| v2ray                |       ✅      |      ✅     |    ❌    |
| SSR                  |       ✅      |      ✅     |    ❌    |
| Eclipse              |       ❌      |      ❌     |    ✅    |
| Ease of Use          |       ✅      |     🟨     |    🟨   |
| Speed                |       ✅      |     🟨     |    🟧   |
| Stability            |       ✅      |      ✅     |    🟨   |
| TCP                  |       ✅      |      ✅     |    ✅    |
| UDP                  |       ✅      |     🟨     |    ✅    |
| Netflix support      |       ✅      |      ✅     |    🟧   |
| Gaming               |       ✅      |     🟨     |    🟧   |

## Android

Recommendation: Latest AnXray. This app supports all our protocols except for OpenVPN. Performance of all apps highly dependent on Phone type, Android version, and CPU.

|                      | AnXray | v2rayNG | ClashR | SSR | OpenVPN |
| -------------------- | :----: | :-----: | :----: | :-: | :-----: |
| Officially supported |    ✅   |    ✅    |    ❌   |  ❌  |    ✅    |
| Trojan               |    ✅   |    ✅    |    ❌   |  ❌  |    ❌    |
| Xray                 |    ✅   |    ✅    |    ❌   |  ❌  |    ❌    |
| v2ray                |    ✅   |    ✅    |    ✅   |  ❌  |    ❌    |
| SSR                  |    ✅   |    ❌    |    ✅   |  ✅  |    ❌    |
| Eclipse              |    ❌   |    ❌    |    ❌   |  ❌  |    ✅    |
| Ease of Use          |    ✅   |    ✅    |    ✅   |  ✅  |    🟨   |
| Speed                |    ✅   |    ✅    |    ✅   |  🟨 |    🟧   |
| Stability            |    ✅   |    ✅    |    ✅   |  🟨 |    🟨   |
| TCP                  |    ✅   |    ✅    |    ✅   |  ✅  |    ✅    |
| UDP                  |    ✅   |    ✅    |    ✅   |  ✅  |    ✅    |
| Netflix support      |    ✅   |    ✅    |    ✅   |  🟨 |    🟧   |
| Gaming               |    ✅   |    🟨   |   🟨   |  🟨 |    🟥   |

## Linux

To be done...

## Routers

Recommendation: OpenWRT with Passwall installed. You can usually get one on taobao, but make sure you ask the seller if Passwall is already installed or not. Otherwise, Merlin-Koolshare routers can be installed later, but they do not support Xray, so we'd recommend trying to get Passwall on OpenWRT if at all possible.

Routers are NOT officially supported. Support provided on a best-effort basis.

If you get a OpenWRT router, it is **HIGHLY, HIGHLY** recommended to get it pre-installed. Installing it yourself is very complicated, if not impossible. We do not provide guides or support on how to install OpenWRT due to the complexity.

{% hint style="info" %}
If you need a router, or have a router but need help installing OpenWRT with all the apps needed, many of our users have had a good experience with @OpenFirmware. You can contact him on telegram via our group chat (mention him @OpenFirmware) or by private message [here](https://t.me/OpenFirmware).
{% endhint %}

|                      | Merlin |                   OpenWRT                   |
| -------------------- | :----: | :-----------------------------------------: |
| Officially supported |    ❌   |                      ❌                      |
| Trojan               |    ✅   |                      ✅                      |
| Xray                 |    ❌   | <p>✅</p><p>Latest </p><p>Passwall only </p> |
| v2ray                |    ✅   |                      ✅                      |
| SSR                  |    ✅   |                      ✅                      |
| Eclipse              |    ✅   |                      ✅                      |
| Installation         |   🟧   |                pre-installed                |
| Ease of Use          |   🟨   |                      ✅                      |
| Speed                |    ✅   |                      ✅                      |
| Stability            |    ✅   |                      ✅                      |
| TCP                  |    ✅   |                      ✅                      |
| UDP                  |   🟨   |                      ✅                      |
| Netflix support      |    ✅   |                      ✅                      |
| Gaming               |    ?   |                      ?                      |

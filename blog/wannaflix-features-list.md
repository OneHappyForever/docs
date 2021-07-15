# WannaFlix Features List

We at WannaFlix are dedicated to give you the best internet experience possible, especially for those of you who are living in countries with internet restrictions.

That's why we have been adding different tools and features to our service over the years. 

But there are now so many of them that it's difficult to keep track of all of them sometimes. So we've created this index of all that WannaFlix offers. Perhaps you will even discover something new and useful!

## Quick list of most common features

* A VPN Proxy running these protocols:

  * v2ray \(VMESS\)
  * xray \(VLESS+XTLS\)
  * ShadowsocksR
  * OpenVPN \( including Eclipse, a slightly tweaked version of OpenVPN that works in China\)
  * SmartDNS

* Apps running on Windows, Mac, iOS, Android, and Merlin/OpenWRT routers

* We have 2 websites:

  * Our main website: [wannaflix.com](https://wannaflix.com)
  * Our China-accessible website: [wannaflix.net](https://wannaflix.net)

* Our website dashboard \(after logging in\) is now available in Chinese \(English being the default\)

* We support Visa/Mastercard, UnionPay, some cryptos, and Alipay

  * NOTE: Alipay works with non-Chinese Alipay accounts too!

* You can contact us in 3 ways:

  * By opening a support ticket \(use wannaflix.net if you can't access wannaflix.com\)
  * By sending us an email at admin@wannaflix.com \(it works from any email address\)
  * Via our [Telegram group chat](https://t.me/wannaflixvpn)

## Account Related

* You can purchase multiple subscriptions under one account \(useful for companies for example\)

  * A dropdown menu will automatically appear once you have more than 1 subscription so you can select the one you want to manage
  * Each subscription has their own Eclipse/SmartDNS subscription too 

* You can register as an affiliate and earn money when people sign up with your link
  * Please send us a ticket if you want to know the commission rate
* You can extend your subscription in advance from the dashboard, even before any invoice has been created

* Invoices are created 14 days before the due date so you have plenty of time to pay them

  * An email will be sent to remind you when the invoice is due

* You can charge your account with credit if you don't want to keep entering your payment details each time.

  * NOTE: You will still need to manually pay the invoice, it'll just be quicker

## App & API Functionality

* Netch uses the same TUN/TAP interface as OpenVPN to capture all traffic

  * This works well with Games
  * Proxy mode is usually faster/more stable

* v2rayN is great for testing which server is working. 

  * You can do speed tests, ping tests, TCP ping tests and real delay tests \(tests whether you can access google\)

* Clash now has a new API! With this new API, you can:

  * Do website split-tunneling, meaning you can have Netflix go via server A, Chinese sites via server B, and all other sites via server C
  * Block Ads
  * Automatically use the fastest server \(switches when another one gets faster or the one you are using stops working\)
  * To get it, login to your dashboard, select your APP from the dropdown, and copy the "Full API"
  * This works on Clash for Windows, ClashX, Clash for Android,  MerlinClash, and OpenClash
  * It does NOT work on ClashR \(android\). Please switch to Clash for Android instead \(you can get it from github or the play store\)

* If your API has been compromised, you can reset it in the dashboard. 
  * NOTE: This will change your VPN password as well, so all your v2ray apps will stop working until you add the servers back in via the new API

## Telegram

* We have 2 Telegram channels:

  * Our [group chat](https://t.me/wannaflixvpn)
  * Our [News/Update channel](https://t.me/wannaflix) were we post important information regarding updates, upgrades, or server issues
  * You can subscribe to our news channel to be notified of our latest updates

* We know the Telegram requires a VPN, which is annoying when you need help when your VPN stopped working. So we provide a Telegram proxy that you can use even when the VPN doesn't work.

  * Click [here ](https://t.me/socks?server=wannaflix.teacher2070.com&port=62000&user=wannaflix&pass=wannaflix.com)to add it now

## Other Tools \(lesser known quick list\)

* A [free seedbox!](https://wannaflix.com/torrenting.php)

* All v2ray servers that do NOT natively unblock Netflix/Hulu/BBC iPlayer, etc. now unblock them by default
  * If they natively unblock them, we keep the local version
  * Otherwise, we default them to US Netflix
  * All servers with "Netflix" in the name unblock the LOCAL version of Netflix, NOT US Netflix, though they will still unblock BBC iPlayer, etc. which only has 1 region.


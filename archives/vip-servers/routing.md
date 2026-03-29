# Routing

This page will help you select the best server for your needs and aims to provide greater transparancy in the routing of the VIP servers.

{% hint style="info" %}
Abreviations: 

CT: China Telecom

CU: China Unicom

CM: China Mobile

CN2: Premium China Telecom network
{% endhint %}

## From China

#### Hong Kong 1

China Telecom: CT -&gt; China Server CN2 -&gt; Hong Kong PCCW

China Unicom: CU -&gt; CT -&gt; China Server  CN2 -&gt; Hong Kong PCCW

China Mobile: CM -&gt; CT -&gt; China Server CN2 -&gt; Hong Kong PCCW

Ping: 50 ms + time to China Server CN2

#### Hong Kong 2

China Telecom: CT -&gt; China Server CN2 -&gt; Hong Kong PCCW

China Unicom: CU -&gt; CT -&gt; China Server CN2 -&gt; Hong Kong PCCW

China Mobile: CM -&gt; CT -&gt; China Server CN2 -&gt; Hong Kong PCCW

Ping: 40 ms + time to China Server CN2

#### Hong Kong 3 via AMAZON CDN

China Telecom: CT -&gt; Hong Kong AMAZON

China Unicom: CU -&gt; Hong Kong Unicom -&gt; Hong Kong AMAZON

China Mobile: CM -&gt; Hong Kong CMI -&gt; Hong Kong PCCW

Ping: 40-50 ms for CT/CU, ~100 ms for CM

#### Hong Kong 4 via AMAZON CDN

China Telecom: CT -&gt; Hong Kong AMAZON

China Unicom: CU -&gt; Hong Kong Unicom -&gt; Hong Kong AMAZON

China Mobile: CM -&gt; Hong Kong CMI -&gt; Hong Kong PCCW

Ping: 60-70 ms for CT/CU, ~120 ms for CM

#### Japan

China Telecom: CT -&gt; China Server CN2 -&gt; Japan NTT

China Unicom: CU -&gt; CT -&gt; China Server  CN2 -&gt; Japan NTT

China Mobile: CM -&gt; CT -&gt; China Server  CN2 -&gt; Japan NTT

Ping: 65ms + time to China Server CN2 

#### Korea 

China Telecom: CT -&gt; CN2 -&gt; Korea BGP

China Unicom: CU -&gt; CN2 -&gt; Korea BGP

China Mobile: CM -&gt; Hong Kong CMI -&gt; Korea BGP

Ping average: 50 ms on all 3 networks 

Ping range: 30 - 60 ms

#### Singapore

China Telecom: CT -&gt; China Server CN2 -&gt; Singapore PCCW

China Unicom: CU -&gt; CT -&gt; China Server CN2 -&gt; Singapore  PCCW

China Mobile: CM -&gt; CT -&gt; China Server CN2 -&gt; Singapore PCCW

Ping: 70ms + time to China Server CN2

#### US West Coast

China Telecom: CT -&gt; China Server CN2 -&gt; Los Angeles \(Level 3\)

China Unicom: CU -&gt; CT -&gt; China Server CN2 -&gt; Los Angeles \(Level 3\)

China Mobile: CM -&gt; CT -&gt; China Server CN2 -&gt; Los Angeles \(Level 3\)

Ping: 130ms + time to China Server CN2

#### Europe

China Telecom: CT -&gt; China Server CM -&gt; Germany DIRECT

China Unicom: CU -&gt; China Server CM -&gt; Germany DIRECT

China Mobile: CM -&gt; China Server CM -&gt; Germany DIRECT

Ping: 220ms + time to China Server CM

## From Other Countries

Each country will have different routing to the non-\[CHINA\] servers. However, all our servers are well connected to multiple major international networks and provide fast and stable connections no matter where you are.

**Hong Kong 3 & 4 via AMAZON CDN**

Average ping to AMAZON CDN: 2-7 ms + time to Hong Kong

**US West Coast & STREAMING via CLOUDFLARE CDN**

Average ping to CLOUDFLARE CDN: 2-20 ms + time to USA


# IP banning: Proxies

Banning by IP was one of the first kinds of banning that was developed. Most websites around the world are able to **detect those IPs that are abusing the server** (too many requests in a short period) and throttle or directly stop serving the content.

Another kind of IP banning is **by geography**. There are different databases and services that can provide with a high degree of confidence where an IP is coming from, and the website can decide if the content should be delivered to the end user or not.

Recently, the process has been improving, and some websites are able to **detect when an IP comes from a data center or from a real device**, and even **if the IP is coming from a mobile phone network** or not.

For all those reasons, **hiding the real IP has become a must when scraping websites**, and the most common way to do it is by using proxies. 

A **proxy** (or proxy server) is a layer that can be put **in the middle of our scraping software and the website**, making the last one to think that the request has originated in the “proxy” itself. This allows to “simulate” other geographies, and IP characteristics.

It is possible to set up proxies manually, but to properly escalate the process, a lot of proxy IPs are needed, and it is a complex challenge. For that reason, multiple companies have developed their own solutions offered as **“proxy networks”**.


## Types of proxy networks:

Here you will find different types of proxy networks based on the characteristics and origins of their IPs.


### Datacenter proxy
IPs coming from datacenters (servers). Faster than requests going through residential and mobile proxies because the request's journey is shorter and the architecture is simplified.


#### Some variants based on access type:

* **Shared IPs (rotating)**: They are from a pool of shared IPs (used by multiple customers). Something to consider is that when using a “shared proxy”, multiple users use the same proxies at the same time, so the performance is compromised. Also, if one user gets blocked, the other users using the same proxies will suffer the same consequences.
* **Semi-dedicated proxy**: exactly the same as “shared IPs proxies”, but they are limited to a certain number of users. For that reason, the performance is usually better.
* **Shared IPs “static”**: They are from a pool of shared IPs, but you can buy it and reuse it because the IP will always be the same (it will be charged by IP + by GB).
* **Exclusive IPs / Private proxy**: Allows to buy an IP and ensures that you will be the only user of that IP for a target domain.




### ISP Proxy (or “Static” Residential Proxy)
Real residential IPs that allow being perceived as they would have originated from real places of residence. The proxy provider rents them to ISPs.

Possibility of using the same IP for a very long time (no IP rotation). Higher speed than usual residential IPs.



### Residential Proxy (Rotational)
A global network of IPs belonging to real individuals. More effective/undetectable than Datacenter IPs.

They can be from every Country / State / City. 


#### How are they obtained?

Examples:
* **Bright data (formerly Luminati**): Users install an SDK and receive a monthly remuneration based on the offer/demand of IPs. Instead of a money remuneration, they can be also compensated by removing Ads or getting a premium update from some mobile app. Theoretically, users can opt-out when they want. The company's origins are related to the HOLA! free VPN, with which users were able to connect to blocked websites while they give access to their bandwith/IP.
* **Charity engine**: They users install a software that can use their internet connection and unused computing power to raise money for charities.



### Mobile Proxy
Real 3G and 4G proxy connections that are assigned to individuals by their mobile carrier. Real user mobile connections. They can be selected by city/country or even choose the ASN or mobile carrier.




### Proxy Network Types Comparison:
|   | Datacenters Proxy | ISP Proxies | Residential proxies | Mobile proxies |
| --- | --- | --- | --- | --- |
| Speed | Faster | Fast | Low | Low |
| Available geographies | High. Example value: ~95 countries  | Limited. Example value: ~35 countries  | Very High. Example value: ~195 countries  | Very High. Example value: ~195 countries  |
| Available IPs (number) | Reasonable. Example value: 1M  | Reasonable. Example value: 1M  | Very high. Example value: 70M  | High Example- value: 7M IPs  |
| Price | Very cheap. Example value: $0.07/Gb to $0.10/Gb (or even lower if offers unlimited bandwidth and charged by IP)  | Expensive. Example values: $7.50/Gb to $17.50/Gb  | Expensive. Example values: $6.00/Gb to $17.50/Gb  | Very expensive. Example value: $23/Gb to $35/Gb  |
| Detection | High | Low | Low | Low |

Example values are coming from an analysis of some Proxy networks providers.



### Other Proxy Networks approaches

They’ve been some companies developing some solutions build on top of proxy networks that, apart from providing proxy IPs, apply some proprietary algorithms and logic to the requests to avoid detection like specific rotation, retries when ban detecting, fingerprint simulation techniques (like modifying/adapting HTTP Headers, etc), ML algorithms, etc.


They usually charge based on the number of successful requests. They can be a good option when targeting multiple and websites like retail websites.

That’s the case of Zyter Smart Proxy Manager (formerly Crawlera), Next-Gen Residential Proxies (from Oxylabs), and Web Unlocker from Luminati.



## Is there any other way to hide the IP?

Another option to hide the real IP would be using a VPN. Both things (proxies and VPNs) will mask your IP, but there’s a key difference between a Proxy and a VPN: the proxy is just a gateway while the VPN builds a tunnel between the origin and the target website and all data that goes through it is encrypted. 

VPNs are designed to be used by individuals that care about privacy. It is technically possible to use a VPN service to scrape websites, but they are not designed with this purpose in mind and that can produce some difficulties. As the VPN is focused on privacy and performs some actions to encrypt the data, this fact causes significant overall slowdowns since all of the traffic is routed through the VPN server and all data has to be encrypted and decrypted.




## Some well-known proxy providers:

* [Bright data (formerly Luminati)](https://brightdata.com/)
* [Oxylabs](https://oxylabs.io/)
* [Netnut](https://netnut.io/)
* [Geosurf](https://www.geosurf.com)
* [Lime proxies](https://www.limeproxies.com/)
* [Proxyland](https://proxyland.co/)
* [Soax](https://soax.com/)


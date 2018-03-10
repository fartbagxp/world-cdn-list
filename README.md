# Overview

This acts as a curated list of [CDNs](https://en.wikipedia.org/wiki/Content_delivery_network) and locations of their CIDR blocks.

Determining a list of CIDR blocks or IP addresses of CDNs is sort of an impossible problem as companies cycle these addresses in and out, and don't normally publish them.

## Why

Edge nodes with content delivery support closer to customers is increasingly becoming more common.

A coworker and I once had a problem where we had to resolve a particular host, but every time it resolves, it would lead to a different IP address.

The host was backed by [Cloudflare](https://www.cloudflare.com/), and we ended up caching IP address that were previously resolved in a database with an expiration.

It's not an ideal solution, and we could do better if we knew we were being served by a particular CDN.

## Sources

The list of CDN is provided by [Wikipedia](https://en.wikipedia.org/wiki/Content_delivery_network#Notable_content_delivery_service_providers).

It would be nice to automatically build a new list (in JSON) and determine the latest set of CIDR blocks for the CDN.

* [BootstrapCDN / MaxCDN](https://www.maxcdn.com/one/tutorial/ip-blocks/)

* [Cloudflare](https://www.cloudflare.com/ips/)

* JSDelivr (uses StackPath, Cloudflare, Fastly, and Quantil)

* [Incapsula](https://www.imperva.com/ld/incapsula/cloud_waf.asp?ref=&cc=)

* [AT&T Inc.](https://developer.att.com/technical-library/network-technologies/ip-addresses)?

* Bharti Airtel (?)

* Bell Canada (?)

* BT Group (?)

* CenturyLink (?)

* China Telecom
* Deutsche Telekom
* Hibernia Networks
* IP-Only
* KT
* KPN
* Level 3 Communications
* Megafon
* NTT
* Pacnet
* PCCW
* Qualitynet
* SingTel
* SK Broadband
* Tata Communications
* Telecom Argentina
* Telecom Italia
* Spark New Zealand
* Telefonica
* Telenor
* TeliaSonera
* Telin
* Telstra
* Telus
* Turk Telekom
* Verizon
* BitTorrent, Inc.
* Internap
* Pando Networks
* Rawflow
* CDN-Tech
* Cloakfusion
* GlobalDots
* MetaCDN

* [Akamai Technologies](https://security.stackexchange.com/questions/38658/firewall-defined-akamai-ip-range)
* [Amazon CloudFront](https://ip-ranges.amazonaws.com/ip-ranges.json)
* Aryaka
* [Azure CDN](https://blogs.technet.microsoft.com/keithmayer/2013/08/14/windows-azure-datacenter-ip-ranges/#.UwFztPmSxvA)
* CacheFly
* CDN.net
* CDNetworks
* CDN77 - 185.59.220.0/24 ?
* CenterServ
* ChinaCache
* [Cloudflare](https://www.cloudflare.com/ips/)
* Cotendo
* Distil Networks
* EdgeCast Networks
* [Fastly](https://api.fastly.com/public-ip-list)
* Highwinds Network Group
* HP Cloud Services
* Incapsula
* Instart Logic
* Internap
* Inxy.hosting
* Inxyhost.com
* LeaseWeb
* [Limelight Networks](https://ipinfo.io/AS22822)
* Medianova.com[30]
* MetaCDN
* NACEVI
* OnApp
* OVH
* Rackspace Cloud Files
* SpaceCDN.com (?)
* Speedera Networks
* StreamZilla
* Wangsu Science & Technology
* Webscale (?)
* Yottaa

* [Redhat](https://access.redhat.com/articles/1525183)

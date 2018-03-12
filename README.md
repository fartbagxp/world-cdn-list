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

Since a lot of CDNs don't normally publish their listing, one way to figure out their allocated netblocks is to go through whois registration sites such as [IPInfo](https://ipinfo.io) to figure out what it is, but false positives can be made provided it that the allocated blocks could be their entire network, instead of simply the CDN part of a company's business.

## Raw data

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

* [Akamai Technologies](https://security.stackexchange.com/questions/38658/firewall-defined-akamai-ip-range)
* [Alibaba Cloud](https://ipinfo.io/AS45102)
  * [198.11.128.0/18](https://ipinfo.io/AS45102/198.11.128.0/18) is probably Alibaba Cloud's US CDN.
* [Amazon CloudFront](https://ip-ranges.amazonaws.com/ip-ranges.json)
* [Aryaka](https://ipinfo.io/AS111790)
* [Azure CDN](https://blogs.technet.microsoft.com/keithmayer/2013/08/14/windows-azure-datacenter-ip-ranges/#.UwFztPmSxvA)
* [CacheFly](https://ipinfo.io/AS30081)
* CDN.net
* [CDNetworks](https://ipinfo.io/AS36408)
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
* Instart Logic
* Internap
* Inxy.hosting
* Inxyhost.com
* LeaseWeb
* [Limelight Networks](https://ipinfo.io/AS22822)
* Medianova.com
* [MetaCDN](https://support.metacdn.com/hc/en-us/articles/205983486-IP-Address-Ranges-for-MetaCDN-Site-Accelerator)
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

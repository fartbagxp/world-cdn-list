# Overview

This acts as a curated list of [CDNs](https://en.wikipedia.org/wiki/Content_delivery_network) and locations of their CIDR blocks.

Determining a list of CIDR blocks or IP addresses of CDNs is sort of an impossible problem as companies cycle these addresses in and out, and don't normally publish them.

> Why?

Edge nodes with content delivery support closer to customers is increasingly becoming more common.

A coworker and I once had a problem where we had to resolve a particular host to gather traffic statistics from it, but every time it resolves, it would lead to a different IP address.

The host was backed by [Cloudflare](https://www.cloudflare.com/), and we ended up a caching IP address that were previously resolved in a database with an expiration.

It's not an ideal solution, and we could do better if we knew we were being served by a particular CDN.

> Figuring out if we're being served by which CDN

There are multiple ways to go around figuring this out.

A common technique seems to be to look at the DNS record of the website, and determine whether any of the CNAME record corresponds to any of the [CDN fronting domains](https://github.com/WPO-Foundation/webpagetest/blob/master/agent/wpthook/cdn.h).

The problem is keeping the CDN domain list relatively updated. If the list goes outdated, we're shit out of luck.

This seems to be the strategy that a popular [CDN Finder](https://github.com/turbobytes/cdnfinder) takes.

> Figuring out which edge servers we'll be serve by for a particular host

Depending on where a request origins from, the same CDN edge server is likely to provide the response for a given host.

In order to figure out all edge servers, it's probably necessary to have as many request origins (different geographical sites) as there are edge servers.

## IP Sources list

I kept an outdated list of IP sources to figure out all the CIDR blocks that different CDN uses.

It can be found in [IP Sources](./ip-sources.md).

## Domain Name

**You will need a domain name** as Sudobox apps are only accessed via https://appname._yourdomain.com_ The steps below will help you set up a domain and DNS settings for use with Sudobox.

Ports are bound primarily to the internal `Sudobox` docker network, which means they are not visible on the host; you won't be able to connect externally to the apps using `IP:PORT`.

# 1. Domain Provider

Get a domain name from any domain name registry (e.g. [Namecheap](https://Namecheap.com), [Godaddy](https://Godaddy.com), [Namesilo](https://Namesilo.com), etc).

If you already have one, you may skip this step.

_Note: Free domain name providers, such as [Freenom](https://www.freenom.com/), do not support wildcard DNS settings, and paid domain names can be had for less than a dollar per year (see promo deals on various sites). However, you can add them to Cloudflare and not have to worry about it._

If you are planning to use the automatic Cloudflare integration, there are some top-level domains [TLDs] that will not work with it.  Refer to [this page](https://support.cloudflare.com/hc/en-us/articles/360020296512-DNS-Troubleshooting-FAQ).

!!!Note:   "DNS API cannot be used for domains with .cf, .ga, .gq, .ml, or .tk TLDs."
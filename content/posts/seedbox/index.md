+++
date = '2026-07-06T16:14:49+02:00'
draft = false
title = 'Seedbox'
tags = ['seedbox', 'piracy', 'whatbox', 'vpn']
showAuthor = false
+++

While on the topic of piracy *([see my previous post about Massgrave](/posts/massgrave))*, I wan't to talk a little bit about seedboxes, and why I prefer to have on over adding the ARR stack to my homelab. Short answer is VPN and HDD prices.

I decided to go with [Whatbox](https://whatbox.ca/) for no particular reason other than I liked their approach and their website design. I really appreciate a simple design. A bit like [Porkbun](https://porkbun.com/) where I bought my latest domains, but that is a different story.

I've been with Whatbox for almost a year now, and I'm very happy with it.

## What is a Seedbox?

Might have to back up a bit and explain what a seedbox actually is.

A seedbox is a virtual machine that you can use to, well, almost anything, within the rules of the provider ofcourse.

Most people use seedboxes to download and seed torrents or [SABnzbd](https://sabnzbd.org/) for the NZB files, which is the equivalent of a torrent file for the NZB format.

## My stack

What I currently have set up on my seedbox is the following:

> [!NOTE] **Transmission**
> [Fast, Easy and Free Bittorrent Client for macOS, Windows and Linux](https://transmissionbt.com/)
{icon="transmission"}

> [!NOTE] **Jellyfin**
> [Free Software Media System](https://jellyfin.org/)
{icon="jellyfin"}

> [!NOTE] **Prowlarr**
> [The Ultimate Indexer Manager](https://prowlarr.com/)
{icon="prowlarr"}

> [!NOTE] **Radarr**
> [Movie collection manager for Usenet and BitTorrent users](https://radarr.video/)
{icon="radarr"}

> [!NOTE] **Sonarr**
> [TV-show collection manager for Usenet and BitTorrent users](https://sonarr.tv/)
{icon="sonarr"}

## Why a Seedbox?

Let's be honest, you don't need a seedbox to download torrents. You can do it on your own computer, but a seedbox is a convenient and safe way to do it.

Pros and cons of using a seedbox:

> [!TIP] **Pros**
>
> - Your real IP address is not exposed, reducing legal and ISP-related risks.  
> - Access from anywhere with an internet connection, without needing to set up a VPN and risk exposing your IP.
> - Easy management via a web-based interface.  
> - No need for a VPN subscription.  
> - Minimal impact on your local power usage.  
> - High download and upload speeds (often faster than home connections).  
> - Built-in tools like torrent clients, file managers, or media streaming (depends on provider).  
> - Better seeding ratio management, especially for private trackers.
{icon="check"}

> [!WARNING] **Cons**
>
> - Monthly cost varies depending on provider and performance tier.  
> - Limited control compared to self-hosting, even though providers like [Whatbox](https://www.whatbox.ca/) offer decent customization.  
> - Reliance on a third-party service (downtime or policy changes can affect access).  
> - Privacy depends on how much you trust the provider.  
> - Some plans include storage or bandwidth limits.  
{icon="xmark"}

# WIP

---
layout: post
lang: en
title: "How to stream TVB Jade on TiviMate: 2026 setup guide"
date: 2026-10-15 09:00:00 +0800
description: "Honest, paid-by-our-wallet guide for Hong Kong immigrants who want TVB dramas and variety shows."
target: Hong Kong immigrants who want TVB dramas and variety shows
---


# How to stream TVB Jade on TiviMate: M3U import tutorial

> Audience: Hong Kong emigrants in the UK, Australia, Canada, or the US who want to watch TVB Jade 24h live stream on TiviMate. This is a **pure technical tutorial** — it does not evaluate the copyright status of any channel source.

---

## 1. The problem: why "install the app and you still can't see TVB Jade"

TiviMate is the most popular M3U player on Android TV / Fire TV, but **it does not provide any content by itself** — it only reads the playlist you import, displays the EPG, and hands the video stream to the system decoder.

After installing TiviMate, many people discover two issues:

1. **TiviMate does not have "TVB Jade" built in** — it does not include any TV station by default. All content comes from your M3U link.
2. **Finding an M3U link ≠ actually seeing TVB Jade** — many public lists only label "TVB1" / "TVB-1" / "Jade" / "Hong Kong channels". **Whether it is actually the 24h Jade live stream has to be tested.**

The result: **TiviMate looks like an empty channel list after install, or the list has "TVB" but the playback is black, skipping seconds, or the subtitles don't match.**

---

## 2. Before finding an M3U subscription, recognize three kinds of "TVB channels"

Different providers name TVB channels very differently in their M3U lists. **Confirm what you are looking for first**:

| Channel name | Actual content | 24h live? |
|--------------|----------------|-----------|
| TVB Jade (TVB 翡翠台) | TVB main channel: news + HK dramas + variety | Yes |
| TVB Pearl (TVB 明珠台) | TVB English / Mandarin secondary channel | Yes |
| TVB Plus / TVB J2 | Youth-oriented / variety / info channel | Yes |
| myTV SUPER exclusive channels | myTV SUPER App exclusive streams | Not 24h satellite live |

**Only "TVB Jade" is the one older Hong Kong emigrants are used to.** "TVB HK drama on-demand" or "TVB Plus" in a list is a different thing.

---

## 3. Existing options compared

Below are the five paths overseas Hong Kong emigrants use to watch TVB Jade 24h live, as of October 2026. **All prices come from each service's publicly listed rate.**

| Option | Monthly cost | Is TVB Jade 24h live? | Device | Maintenance |
|--------|--------------|------------------------|--------|-------------|
| **TVB Anywhere+ official app** | **$17 CAD/month** or $180/year | Yes (North America) / restricted (other regions) | Smart TV / phone / Apple TV / Fire TV | Low |
| KyLinTV | $19.99-25.99 CAD/month | Yes | Smart TV / set-top box | Low |
| Public GitHub M3U list | $0 | Some have (labeled "TVB" / "Jade") | Any M3U player | Very high (channels die often) |
| Paid M3U subscription | $5-10/month | Usually has (**must confirm before purchase**) | TiviMate / Televizo | Medium |
| myTV SUPER App (Hong Kong version) | 38 HKD/month | Yes, full rights | Requires VPN + HK IP / HK phone number to register | High (account gets blocked easily) |

A few **factual statements** without judging which is better:

1. **TVB Anywhere+ North America** official registration page: 17 CAD/month or 180 CAD/year. **Note**: it only covers TVB's own channels and selected HK dramas — not all of TVB's licensed content. For example, HK horse racing and TVB show replays older than 7 days are not in the Anywhere+ package.
2. **myTV SUPER is the Hong Kong local version**, **38 HKD/month, overseas IPs are rejected**. Overseas Hong Kong emigrants who want myTV SUPER need a VPN + HK phone number + HK bank or FPS payment — **this path deters over 90% of people**.
3. **M3U (*.m3u / *.m3u8) is a public playlist file format**. Anyone can generate, share, or modify it. **The format itself is just a technical specification and does not bind to any specific channel or content source.** Whether an M3U subscription service is legitimate depends on whether its content source is authorized.
4. **KyLinTV's "Cantonese Pack" is in the base pack** — but **not all base packs include it**. Confirm with support which Cantonese channels are included before purchase.

---

## 4. Technical path: TiviMate + subscription link

### Hardware (one-time)

- **Amazon Fire TV Stick 4K Max**: US $89.48, Canada about $119 CAD (as of October 2026). TiviMate runs most stably on Fire TV.
- **NVIDIA Shield TV Pro**: US $199, Canada about $279 CAD. Stronger performance, but Fire TV Stick 4K Max is enough for most scenarios.
- **Any Android TV smart TV** (Sony, TCL, Hisense): Google Play is built in, install TiviMate directly.

What not to buy:

- **Prepaid set-top boxes marketed as "Asian TV" or "HK/TW TV"** (UBOX, EVPad, SviCloud, etc.): the hardware itself is a cheap Android box — the real dependency is the M3U subscription inside. The provider can stop selling at any time, the box becomes a brick, no after-sales support.
- Any M3U subscription that requires "you must use our box to work": a good subscription should be a URL that works on any device you own.

### Software: M3U player

**An M3U player only reads the playlist, displays the EPG, and sends playback requests.** It does not provide any content itself — all content comes from the M3U link you import.

| Platform | Recommended player | Notes |
|----------|-------------------|-------|
| Android TV / Fire TV / Shield | **TiviMate** | UI closest to traditional cable TV EPG; tivimate.com explicitly states "TiviMate is a media player only and does not provide any content" |
| Android TV / Fire TV / Shield | **Televizo** | Google Play 4.0 rating / 17.7K reviews (com.ottplay.ottplay); modern UI, multiple playlists; free version works, PRO subscription unlocks 5 devices / ad-free |
| iOS / iPadOS / Apple TV | **Smarters IPTV Player** | Listed on the App Store, developer Smarters; also only reads M3U links, no content |
| iOS / iPadOS / Apple TV | **APTV** | Listed on the App Store (id 1630403500), developer Kimen; supports iPhone / iPad / Mac / Apple TV / Apple Watch / Vision Pro across six Apple platforms + CarPlay video casting |
| Any platform | **VLC media player** | Free and open source, supports M3U; but does not render EPG guide, you need to organize channels yourself |

### TiviMate configuration steps

TiviMate on Google Play is free to import M3U. **The full feature set (EPG rendering, recording, multi-device sync) requires an In-App Purchase subscription**. **The developer does not publish a unified subscription price** (as of October 2026); confirm in-app before purchase.

1. **Install TiviMate**: on Fire TV, open Google Play, search "TiviMate", developer is AR Mobile Development. Or download the sideload APK from tivimate.com/apk.
2. **Prepare the M3U subscription link**: usually a URL you get from a paid subscription via email or backend, shaped like `https://example.com/sub/your-code.m3u`. **Only subscribe to a service that explicitly lists TVB Jade in its lineup** — search "TVB Jade" or "Jade" in the provider's channel list before purchase.
3. **Configure the M3U link**: open TiviMate → Settings → My Playlists → Add playlist from URL, paste the link → save.
4. **Wait for the list to load** (usually 10-30 seconds), channel count may be from a few hundred to a few thousand.
5. **Search for TVB channels**: type "TVB" in the channel list's top search box, add **TVB Jade**, **TVB Pearl**, **TVB Plus / J2** to favorites.
6. **Configure the EPG** (optional but recommended): TiviMate → Settings → EPG → Add EPG source, usually the M3U subscription provider also offers an XMLTV-format EPG link — paste it in. **With EPG, the UI looks like traditional cable TV** — browse the schedule to see what's on at 8 PM tonight.
7. **Test stability**: Hong Kong prime time (Beijing 8-10 PM = US ET 7-9 AM / US PT 4-6 AM) is the real-world test scenario.

**For iOS / iPadOS / Apple TV users** use Smarters IPTV Player or APTV — the configuration flow is the same (Smarters: bottom Login → Add User via M3U URL; APTV: bottom Sources → Add Source → M3U URL).

### For parents

After setup, give parents a simplified remote guide:

- **Left/right keys**: switch channels (you pre-place TVB Jade, TVB Pearl, TVB Plus in the top 3 favorites).
- **Up/down keys**: change channel.
- **OK key**: enter the EPG.
- **Back key**: return to the main screen.

**Do not let parents touch the M3U link or subscription renewal.** TiviMate has a "Parental Control / PIN" feature; once enabled, they cannot accidentally delete the playlist. Televizo also supports PIN lock.

---

## 5. FAQ

**Q1: How much does TiviMate cost?**

A: TiviMate is free to download; subscription price is shown inside the Google Play app. **The developer does not publish a unified price list** — prices may differ by region and time. Confirm in-app before purchase.

**Q2: The M3U list has "TVB" but playback is black — what do I do?**

A: Three common reasons:

1. **The link in the M3U list has expired** (upstream CDN changed the URL) — ask the provider for the latest link.
2. **The channel has a region restriction** (e.g., some TVB streams only allow Hong Kong IPs to play) — try binding a proxy in TiviMate for that channel.
3. **Your M3U provider simply does not have the TVB Jade 24h live stream** — only "Jade on-demand" or "HK drama replay", **not real 24h satellite live**. In this case switch providers.

**Q3: Can I watch TVB Anywhere+ inside TiviMate?**

A: No. TVB Anywhere+ is a closed app and does not expose an M3U link. **It uses its own DRM-encrypted stream**, which TiviMate cannot read. Either watch it in the TVB official app, or go the M3U subscription path — **the two cannot be merged**.

**Q4: Where does the EPG data come from?**

A: EPG is a separate data stream, **disconnected from M3U**. Common sources:

1. **Bundled with the M3U provider** (usually the M3U link has an XMLTV link below it, paste into TiviMate's EPG settings).
2. **Public EPG sources** (such as community-maintained sources at epg.iptvx.top) — quality varies, **some sources require payment**.
3. **DIY with xmltv-grabber** — high technical threshold, not recommended for non-technical users.

**Q5: Does TiviMate's recording work?**

A: TiviMate Premium's "recording" is **client-level** — it caches the live stream in real time to the Fire TV Stick's local storage (32GB model has about 14GB usable, **about 6-8 hours of SD / 3-4 hours of HD**). **Not DVR-server-level recording** — no remote scheduling, no remote viewing.

---

## 6. Conclusion

For the need of "watching TVB Jade 24h live on TiviMate", **the most stable 2026 setup is**:

- **Hardware**: Amazon Fire TV Stick 4K Max ($89.48 USD, one-time)
- **Player**: TiviMate (Android); iOS users use APTV or Smarters IPTV Player
- **Subscription**: $5-10 USD/month M3U subscription — **confirm the channel list has TVB Jade (labeled "TVB Jade") before purchase**
- **EPG**: ask the provider for an XMLTV link and paste it into TiviMate → Settings → EPG
- **VPN**: not needed (M3U path); TVB official app does not need it

For households that want **fully compliant, no M3U**, use the TVB Anywhere+ official app directly — **but accept that the North America version has less content than the Hong Kong version**.

---

## 7. Commercial services

This article does not sell any subscription service.

If you want to skip the frequent failures of GitHub lists and the manual M3U configuration process, you can check the GitHub project home page (the **"Commercial services"** section in the `README`) for the author's paid subscription configuration: a maintained TVB Jade / Pearl / J2 channel list, auto-renewing subscription link, and a 7-day trial entry.

> All prices and feature descriptions in this article come from each service's public page as of October 2026 and may change at any time. Confirm on the official website at the time of purchase.
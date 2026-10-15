# Overseas Chinese TV Guide

> Honest, paid-by-our-wallet guides for Chinese-speaking families abroad.

A static site (Jekyll + GitHub Pages) covering the most common "Chinese TV abroad" questions: sports, Cantonese, Hong Kong dramas, Phoenix TV, and budget M3U subscriptions.

## Why this site exists

If you are an overseas Chinese, you have probably run into one of these problems:

- Your parents want Chinese-language sports commentary (NBA, Premier League, World Cup).
- A Cantonese-speaking elder in the family wants Hong Kong dramas.
- You want to keep up with Phoenix TV's news and current affairs.
- You want a stable, cheap way to watch Chinese TV without the prepaid boxes that die in a year.

This site walks through each scenario step by step, with the real 2026 prices, real player setup, and zero marketing.

## What's in it

| Guide | Audience |
|-------|----------|
| [How to watch CCTV-5 in USA]({{ '/2026/10/15/how-to-watch-cctv5-usa-2026.html' | relative_url }}) | US-based Chinese families |
| [Best Chinese TV for Cantonese speakers in Canada]({{ '/2026/10/15/best-iptv-cantonese-canada.html' | relative_url }}) | Cantonese-speaking elders in Toronto / Vancouver |
| [How to stream TVB Jade on TiviMate]({{ '/2026/10/15/stream-tvb-jade-tivimate.html' | relative_url }}) | Hong Kong immigrants |
| [Watch Phoenix TV abroad: M3U vs Sling vs KyLinTV]({{ '/2026/10/15/phoenix-tv-abroad-comparison.html' | relative_url }}) | Anyone who wants Phoenix Info News or Phoenix Chinese |
| [Cheap M3U subscription 2026]({{ '/2026/10/15/cheap-m3u-subscription-2026.html' | relative_url }}) | Overseas Chinese on a budget |

Chinese versions of all five guides are also available in the [archive]({{ '/archive/' | relative_url }}).

## Site policies

1. **No copyrighted material** is hosted on this site. All content is original, paid-for-our-wallet testing notes.
2. **All prices and feature descriptions** come from each service's public page as of October 2026 and may change.
3. **No personal information** is collected on this site. There are no analytics scripts, no cookies, no tracking.

## Commercial services

This site is **not** a store. It does not sell subscriptions, boxes, or hardware.

If you want to skip the manual M3U configuration described in every guide above, the author maintains a paid subscription service with:

- A maintained Chinese channel list (regularly updated as upstream URLs change)
- Auto-renewing subscription link
- A 7-day trial entry to test the channel list before paying

**To learn more, see the [iptv-search.com](https://iptv-search.com) website or contact the author via the GitHub issues page.**

> The author does not control the copyright status of any third-party content. Whether your personal viewing is legal depends on whether the M3U link's content has been authorized by the rights holder. This site does not evaluate any specific service's content source.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000/overseas-chinese-tv-guide/

## License

Site content (Markdown files in `_posts/`) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Code (Jekyll config, layouts, CSS) is licensed under MIT.
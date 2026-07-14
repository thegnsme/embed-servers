# 🎬 Movie & TV Embed Servers — Master List

> Comprehensive directory of video embed servers, APIs, and streaming sources.
> All accept **TMDB ID** or **IMDB ID** (tt-prefixed) unless noted. Format:
> `<iframe src="URL" ...>` embed pattern.

---

## 📋 Table of Contents

1. [🥇 Major Embed API Providers](#-major-embed-api-providers)
2. [🔌 Multi-Server Aggregators](#-multi-server-aggregators)
3. [🧩 Individual Source Servers](#-individual-source-servers)
4. [📦 Self-Hosted / Open Source APIs](#-self-hosted--open-source-apis)
5. [🗂️ Video Hosting Backend Servers](#️-video-hosting-backend-servers)
6. [🛠️ Tools & Wordpress Plugins](#️-tools--wordpress-plugins)

---

## 🥇 Major Embed API Providers

Primary embed services — drop an iframe, get a player.

### VidPlus

| Property        | Value                                                 |
| --------------- | ----------------------------------------------------- |
| **Website**     | [vidplus.to](https://vidplus.to)                      |
| **GitHub**      | [vidbox1/vidplus](https://github.com/vidbox1/vidplus) |
| **Player Base** | `https://player.vidplus.to/embed/`                    |

**Endpoints:**

```
Movie:  https://player.vidplus.to/embed/movie/{tmdbId}
TV:     https://player.vidplus.to/embed/tv/{tmdbId}/{season}/{episode}
Anime:  https://player.vidplus.to/embed/anime/{anilistId}/{episode}?dub={true/false}
```

**Parameters:** `autoplay`, `autonext`, `primarycolor`, `secondarycolor`,
`iconcolor`, `server`, `poster`, `title`, `chromecast`, `watchparty`,
`progress`, `hideposter`, `hidetitle`, `hidechromecast`, `hidepip`,
`hideepisodelist`, `hideservericon`, `font`, `fontcolor`, `fontsize`, `opacity`,
`logourl`, `icons`

| Example | URL                                                                                            |
| ------- | ---------------------------------------------------------------------------------------------- |
| Movie   | [`https://player.vidplus.to/embed/movie/27205`](https://player.vidplus.to/embed/movie/27205)   |
| TV      | [`https://player.vidplus.to/embed/tv/94997/1/1`](https://player.vidplus.to/embed/tv/94997/1/1) |
| Anime   | [`https://player.vidplus.to/embed/anime/21/1`](https://player.vidplus.to/embed/anime/21/1)     |

---

### VidLux

| Property        | Value                                                                                   |
| --------------- | --------------------------------------------------------------------------------------- |
| **Website**     | [vidlux.site](https://vidlux.site)                                                      |
| **Docs**        | [vidlux.site/docs](https://vidlux.site/docs)                                            |
| **GitHub**      | [segseaweber/vidlux-streaming-api](https://github.com/segseaweber/vidlux-streaming-api) |
| **Player Base** | `https://vidlux.site/embed/`                                                            |

**Endpoints:**

```
Movie:  https://vidlux.site/embed/movie/{tmdbId}?key={API_KEY}
TV:     https://vidlux.site/embed/tv/{tmdbId}/{season}/{episode}?key={API_KEY}
```

**Servers:** Alpha, Nova, Astra, Flix, Delta, Omega (HLS/MP4)

**Parameters:** `key` (required), `color`, `autoplay`, `server`

| Example | URL                                                                                                 |
| ------- | --------------------------------------------------------------------------------------------------- |
| Movie   | [`https://vidlux.site/embed/movie/603692?key=YOUR_API_KEY`](https://vidlux.site/embed/movie/603692) |
| TV      | [`https://vidlux.site/embed/tv/1399/1/1?key=YOUR_API_KEY`](https://vidlux.site/embed/tv/1399/1/1)   |

---

### VidSrc (Primary Domain Network)

| Property          | Value                                                                                                                                                                                                                       |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Domain Status** | [vidsrc.domains](https://vidsrc.domains)                                                                                                                                                                                    |
| **Live Domains**  | [vidsrcme.ru](https://vidsrcme.ru) · [vsrc.su](https://vsrc.su) · [vidsrc-embed.ru](https://vidsrc-embed.ru) · [vidsrc-me.ru](https://vidsrc-me.ru) · [vidsrc.fyi](https://vidsrc.fyi) · [vidsrc.wiki](https://vidsrc.wiki) |
| **Old Domains**   | vidsrc.me · vidsrc.to · vidsrc.io · vidsrc.bz · vidsrc.gd · vidsrc.do · vidsrc.tw                                                                                                                                           |
| **Community**     | [vidsrc.community](https://vidsrc.community)                                                                                                                                                                                |

**Endpoints (applies to all domains):**

```
Movie:  https://{domain}/embed/movie/{id}
TV:     https://{domain}/embed/tv/{id}/{season}/{episode}
```

**vidsrc.fyi extra API:**

```
Movie List:   https://vidsrc.fyi/vapi/movie/{type}/{page}   (type: new, add)
TV List:      https://vidsrc.fyi/vapi/tv/{type}/{page}
Episodes:     https://vidsrc.fyi/vapi/episode/latest
```

| Example      | URL                                                                                      |
| ------------ | ---------------------------------------------------------------------------------------- |
| Movie (fyi)  | [`https://vidsrc.fyi/embed/movie/tt17048514`](https://vidsrc.fyi/embed/movie/tt17048514) |
| Movie (wiki) | [`https://vidsrc.wiki/embed/movie/533535`](https://vidsrc.wiki/embed/movie/533535)       |
| TV (fyi)     | [`https://vidsrc.fyi/embed/tv/tt0944947/1/5`](https://vidsrc.fyi/embed/tv/tt0944947/1/5) |
| TV (wiki)    | [`https://vidsrc.wiki/embed/tv/1399/1/1`](https://vidsrc.wiki/embed/tv/1399/1/1)         |

**Custom color:**
[`https://v2.vidsrc.me/embed/tt1300854/color-15006D`](https://v2.vidsrc.me/embed/tt1300854/color-15006D)

**Parameters:** `?autoplay=1`, `?color=e50914`, `?sub=en`, `?t=120`,
`?controls=0`, `?sub.info={json}`

---

### VidCore

| Property        | Value                              |
| --------------- | ---------------------------------- |
| **Website**     | [vidcore.org](https://vidcore.org) |
| **Docs**        | [vidcore.org](https://vidcore.org) |
| **Player Base** | `https://vidcore.org/embed/`       |

**Endpoints:**

```
Movie:  https://vidcore.org/embed/movie/{tmdbId}
TV:     https://vidcore.org/embed/tv/{tmdbId}/{season}/{episode}
```

**Parameters:** `autoPlay`, `title`, `poster`, `startAt`, `theme` (hex),
`server`, `hideServer`, `fullscreenButton`, `chromecast`, `sub`

| Example              | URL                                                                                                          |
| -------------------- | ------------------------------------------------------------------------------------------------------------ |
| Movie                | [`https://vidcore.org/embed/movie/533535`](https://vidcore.org/embed/movie/533535)                           |
| Movie (custom theme) | [`https://vidcore.org/embed/movie/533535?theme=FF0000`](https://vidcore.org/embed/movie/533535?theme=FF0000) |

---

### 2Embed

| Property        | Value                                                                   |
| --------------- | ----------------------------------------------------------------------- |
| **Website**     | [2embed.online](https://www.2embed.online)                              |
| **Alt Domains** | [2embed.cc](https://2embed.cc) · [2embed.stream](https://2embed.stream) |
| **Player Base** | `https://www.2embed.online/embed/`                                      |

**Endpoints:**

```
Movie:           https://www.2embed.online/embed/movie/{id}
TV:              https://www.2embed.online/embed/tv/{id}/{season}/{episode}
Auto-detect:     https://www.2embed.online/iframe.php?id={id}
```

| Example      | URL                                                                                                    |
| ------------ | ------------------------------------------------------------------------------------------------------ |
| Movie (IMDB) | [`https://www.2embed.online/embed/movie/tt23779058`](https://www.2embed.online/embed/movie/tt23779058) |
| Movie (TMDB) | [`https://www.2embed.online/embed/movie/1147301`](https://www.2embed.online/embed/movie/1147301)       |
| TV           | [`https://www.2embed.online/embed/tv/205715/1/1`](https://www.2embed.online/embed/tv/205715/1/1)       |
| Auto-detect  | [`https://www.2embed.online/iframe.php?id=1029880`](https://www.2embed.online/iframe.php?id=1029880)   |

---

### SuperEmbed / MultiEmbed

| Property        | Value                                              |
| --------------- | -------------------------------------------------- |
| **Website**     | [superembed.stream](https://www.superembed.stream) |
| **Player Base** | `https://multiembed.mov/`                          |

**Endpoints:**

```
Movie (IMDB):  https://multiembed.mov/?video_id={imdbId}
Movie (TMDB):  https://multiembed.mov/?video_id={tmdbId}&tmdb=1
TV (IMDB):     https://multiembed.mov/?video_id={imdbId}&s={season}&e={episode}
TV (TMDB):     https://multiembed.mov/?video_id={tmdbId}&tmdb=1&s={season}&e={episode}
```

**VIP Player (ad-light):**

```
VIP Movie:     https://multiembed.mov/directstream.php?video_id={id}
VIP TV:        https://multiembed.mov/directstream.php?video_id={id}&s={season}&e={episode}
VIP Check:     Add &check=1  (returns 0/1)
Custom Subs:   &sub_url={url}&sub_label={label}
```

| Example      | URL                                                                                                                        |
| ------------ | -------------------------------------------------------------------------------------------------------------------------- |
| Movie        | [`https://multiembed.mov/?video_id=tt8385148`](https://multiembed.mov/?video_id=tt8385148)                                 |
| Movie (TMDB) | [`https://multiembed.mov/?video_id=522931&tmdb=1`](https://multiembed.mov/?video_id=522931&tmdb=1)                         |
| TV           | [`https://multiembed.mov/?video_id=tt13157618&s=1&e=2`](https://multiembed.mov/?video_id=tt13157618&s=1&e=2)               |
| VIP Movie    | [`https://multiembed.mov/directstream.php?video_id=tt6791350`](https://multiembed.mov/directstream.php?video_id=tt6791350) |

---

### Embed-API

| Property        | Value                                        |
| --------------- | -------------------------------------------- |
| **Website**     | [embed-api.stream](https://embed-api.stream) |
| **Player Base** | `https://player.embed-api.stream/`           |

**Endpoints:**

```
Movie:  https://player.embed-api.stream/?id={tmdbId}
TV:     https://player.embed-api.stream/?id={tmdbId}&s={season}&e={episode}
```

**Aggregated servers:** MoviesAPI, VidZee, Vidify, VidRock, MappleTV, VidLink,
PrimeWire, MultiEmbed, VidBinge, VidSrc, AutoEmbed, 2Embed

| Example | URL                                                                                                      |
| ------- | -------------------------------------------------------------------------------------------------------- |
| Movie   | [`https://player.embed-api.stream/?id=786892`](https://player.embed-api.stream/?id=786892)               |
| TV      | [`https://player.embed-api.stream/?id=76479&s=4&e=1`](https://player.embed-api.stream/?id=76479&s=4&e=1) |

---

### Vidify

| Property        | Value                              |
| --------------- | ---------------------------------- |
| **Player Base** | `https://player.vidify.top/embed/` |

**Endpoints:**

```
Movie:  https://player.vidify.top/embed/movie/{tmdbId}
TV:     https://player.vidify.top/embed/tv/{tmdbId}/{season}/{episode}
```

**Parameters:** `ad`, `primaryColor`, `secondaryColor`, `iconColor`, `autoplay`,
`poster`, `chromecast`, `servericon`, `setting`, `pip`, `font`, `fontcolor`,
`fontsize`, `opacity`, `logourl`, `server`

| Example | URL                                                                                          |
| ------- | -------------------------------------------------------------------------------------------- |
| Movie   | [`https://player.vidify.top/embed/movie/12345`](https://player.vidify.top/embed/movie/12345) |

---

### SmashyStream

| Property        | Value                           |
| --------------- | ------------------------------- |
| **Player Base** | `https://player.smashy.stream/` |

**Endpoints:**

```
Movie:  https://player.smashy.stream/movie/{id}
TV:     https://player.smashy.stream/tv/{id}?s={season}&e={episode}
```

**Parameters:** `btPosition`, `playerList`, `remove`, `startTime`, `subLang`

| Example | URL                                                                                                      |
| ------- | -------------------------------------------------------------------------------------------------------- |
| Movie   | [`https://player.smashy.stream/movie/tt4154796`](https://player.smashy.stream/movie/tt4154796)           |
| TV      | [`https://player.smashy.stream/tv/tt0903747?s=1&e=5`](https://player.smashy.stream/tv/tt0903747?s=1&e=5) |

---

### PrimeSrc

| Property    | Value                              |
| ----------- | ---------------------------------- |
| **Website** | [primesrc.me](https://primesrc.me) |
| **Library** | 77,000+ movies · 275,000+ episodes |

**Endpoints:**

```
Movie:  https://primesrc.me/embed/movie/{id}
TV:     https://primesrc.me/embed/tv/{id}?sea={season}&epi={episode}
```

Supports IMDb, TMDB, and TVMaze IDs. 14+ file hosting servers aggregated. Built
with Elixir/Phoenix + Cloudflare.

---

### EmbedMaster

| Property    | Value                                                                   |
| ----------- | ----------------------------------------------------------------------- |
| **Website** | [embedmaster.com](https://embedmaster.com)                              |
| **Docs**    | [embedmaster.com/documentation](https://embedmaster.com/documentation/) |

Requires registration / API key. Features: 10+ streaming servers (StreamTape,
DoodStream, FlixHQ, StreamWish, MixDrop, Abyss, EarntVids, SaveFiles, BigWarp,
FileMoon, VidMoly, VOE), 4K streaming, ad-free option, custom branding.

---

### NontonGo

| Property    | Value                                    |
| ----------- | ---------------------------------------- |
| **Website** | [nontongo.win](https://www.nontongo.win) |

**Endpoints:**

```
Movie (IMDB):  https://www.nontongo.win/embed/movie/{imdbId}
Movie (TMDB):  https://www.nontongo.win/embed/movie/{tmdbId}
TV (IMDB):     https://www.nontongo.win/embed/tv/{imdbId}/{season}/{episode}
TV (TMDB):     https://www.nontongo.win/embed/tv/{tmdbId}/{season}/{episode}
TV (alt):      https://www.nontongo.win/embed/tv/?id={id}&s={season}&e={episode}
Anime:         https://nontongo.win/embed/anime/{slug}
```

| Example | URL                                                                                                            |
| ------- | -------------------------------------------------------------------------------------------------------------- |
| Movie   | [`https://www.nontongo.win/embed/movie/tt6806448`](https://www.nontongo.win/embed/movie/tt6806448)             |
| TV      | [`https://www.nontongo.win/embed/tv/tt0903747/1/1`](https://www.nontongo.win/embed/tv/tt0903747/1/1)           |
| Anime   | [`https://nontongo.win/embed/anime/one-piece-episode-1`](https://nontongo.win/embed/anime/one-piece-episode-1) |

---

### VIDEmbed (myflixerapi)

| Property        | Value                                                        |
| --------------- | ------------------------------------------------------------ |
| **Website**     | [vidsrc.myflixerapi.com](https://vidsrc.myflixerapi.com/api) |
| **Player Base** | `https://vidsrc.myflixerapi.com/embed/`                      |

**Endpoints:**

```
Movie (IMDB):  https://vidsrc.myflixerapi.com/embed/movie?imdb={id}
Movie (TMDB):  https://vidsrc.myflixerapi.com/embed/movie?tmdb={id}
Movie (title): https://vidsrc.myflixerapi.com/embed/movie?title={title}&year={year}
TV (IMDB):     https://vidsrc.myflixerapi.com/embed/series?imdb={id}&sea={s}&epi={e}
TV (TMDB):     https://vidsrc.myflixerapi.com/embed/series?tmdb={id}&sea={s}&epi={e}
TV (IDs):      https://vidsrc.myflixerapi.com/embed/{tvImdbId}/{season}/{episode}
Download:      Replace "embed" with "download" in any URL
Server param:  ?server=dood.so
Status check:  https://vidsrc.myflixerapi.com/api/status?imdb={id}&type=movie
```

---

### EzVidApi

| Property    | Value                                |
| ----------- | ------------------------------------ |
| **Website** | [ezvidapi.com](https://ezvidapi.com) |

Free movie & TV streaming API by TMDB ID. Drop-in iframe player and HLS stream
URLs. Multi-provider auto-failover. No API key required.

---

## 🔌 Multi-Server Aggregators

These are the sources that major embed APIs scrape from.

| Server               | Notes                                   | Docs / Source                                             |
| -------------------- | --------------------------------------- | --------------------------------------------------------- |
| **MoviesAPI**        | Aggregated by Embed-API                 | —                                                         |
| **MultiEmbed**       | Aggregated by many providers            | [multiembed.com](https://multiembed.com)                  |
| **AutoEmbed**        | Aggregated by Embed-API, CinePro        | —                                                         |
| **AutoEmbedApp**     | Embed server                            | —                                                         |
| **VidBinge**         | Aggregated by Embed-API, CinePro        | —                                                         |
| **VidSrcMov**        | VidSrc variant                          | —                                                         |
| **VidSrcCC**         | Alternative VidSrc                      | —                                                         |
| **CineSrc**          | Embed server                            | —                                                         |
| **AnyEmbed**         | Embed server                            | —                                                         |
| **StreamMafia**      | Embed server                            | —                                                         |
| **VidKing**          | Embed server                            | —                                                         |
| **Videasy**          | Open source, 10 servers via enc-dec.app | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **Vidzee**           | Aggregated by Embed-API                 | —                                                         |
| **VidLink**          | Embed server, open source               | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **111Movies**        | Embed server                            | —                                                         |
| **Vidfast**          | Embed server                            | —                                                         |
| **Vidrock**          | Aggregated by Embed-API                 | —                                                         |
| **Vidstorm**         | Embed server                            | —                                                         |
| **Peachify**         | Embed server                            | —                                                         |
| **Vembed**           | Embed server                            | —                                                         |
| **MegaEmbed**        | Embed server                            | —                                                         |
| **MappleTV**         | Aggregated by Embed-API                 | —                                                         |
| **PrimeWire**        | Legacy provider, aggregated by CinePro  | —                                                         |
| **Xprime**           | Premium source aggregation              | [GitHub](https://github.com/cinepro-org/backend)          |
| **LordFlix**         | 9 servers via enc-dec.app               | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **Showbox / FebBox** | Requires FebBox JWT cookie              | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **4KHDHub**          | 4K streams                              | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **VixSrc**           | Streams                                 | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **NoTorrent**        | Stremio addon API                       | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **DahmerMovies**     | Direct file links                       | [GitHub](https://github.com/Inside4ndroid/TMDB-Embed-API) |

---

## 🧩 Individual Source Servers

These are file hosts / video servers that power the embed APIs above.

| Server         | Type      | URL                                      |
| -------------- | --------- | ---------------------------------------- |
| **StreamTape** | File host | [streamtape.com](https://streamtape.com) |
| **DoodStream** | File host | [doodstream.com](https://doodstream.com) |
| **MixDrop**    | File host | [mixdrop.co](https://mixdrop.co)         |
| **FileMoon**   | File host | [filemoon.org](https://filemoon.org)     |
| **VidMoly**    | File host | [vidmoly.me](https://vidmoly.me)         |
| **VOE**        | File host | [voe.sx](https://voe.sx)                 |
| **StreamSB**   | File host | [streamsb.net](https://streamsb.net)     |
| **UpStream**   | File host | [upstream.to](https://upstream.to)       |
| **Abyss**      | File host | [abyss.to](https://abyss.to)             |
| **StreamHide** | File host | [streamhide.to](https://streamhide.to)   |
| **BigWarp**    | File host | [bigwarp.io](https://bigwarp.io)         |
| **SaveFiles**  | File host | —                                        |
| **EarnVids**   | File host | —                                        |
| **FlixHQ**     | File host | —                                        |
| **StreamWish** | File host | [streamwish.to](https://streamwish.to)   |
| **VidStream**  | File host | —                                        |
| **MyCloud**    | File host | —                                        |
| **VidCloud**   | File host | —                                        |

---

## 📦 Self-Hosted / Open Source APIs

### TMDB Embed API

| Property    | Value                                                                           |
| ----------- | ------------------------------------------------------------------------------- |
| **GitHub**  | [Inside4ndroid/TMDB-Embed-API](https://github.com/Inside4ndroid/TMDB-Embed-API) |
| **License** | MIT                                                                             |
| **Stack**   | Node.js, Express                                                                |
| **Docker**  | `inside4ndroid/tmdb-embed-api`                                                  |

**Built-in providers:** Showbox, 4KHDHub, VixSrc, Videasy, VidLink, LordFlix,
NoTorrent, DahmerMovies

**Endpoints (self-hosted):**

```
Health:       GET /api/health
Metrics:      GET /api/metrics
Streams:      GET /api/streams/{type}/{tmdbId}       (type: movie|tv)
Streams/prov: GET /api/streams/{provider}/{type}/{tmdbId}
Config:       GET/POST /api/config
```

### CinePro Backend

| Property   | Value                                                         |
| ---------- | ------------------------------------------------------------- |
| **GitHub** | [cinepro-org/backend](https://github.com/cinepro-org/backend) |
| **Stack**  | Node.js, Express                                              |
| **Docker** | Ready                                                         |

**Providers:** VidSrc, VidSrcCC, MultiEmbed, AutoEmbed, Xprime, PrimeWire

**Endpoints (self-hosted):**

```
Movie:   GET /movie/{tmdbId}
TV:      GET /tv/{tmdbId}?s={season}&e={episode}
Cache:   GET /cache-stats
```

### VidSrc Scraper

| Property   | Value                                                                       |
| ---------- | --------------------------------------------------------------------------- |
| **GitHub** | [DivineChile/vidsrc-scraper](https://github.com/DivineChile/vidsrc-scraper) |
| **Stack**  | Node.js, Express, Playwright                                                |

Scrapes HLS .m3u8 and subtitles from multiple VidSrc domains.

### Stremsrc

| Property   | Value                                                     |
| ---------- | --------------------------------------------------------- |
| **GitHub** | [ThEditor/stremsrc](https://github.com/ThEditor/stremsrc) |

Stremio addon that aggregates VidSrc domains with fallback rotation.

---

## 🗂️ Video Hosting Backend Servers

These are the underlying streaming servers that the embed APIs proxy/scrape:

| Server             | Type               | Notes                              |
| ------------------ | ------------------ | ---------------------------------- |
| **GDrive Player**  | Google Drive proxy | Used by older embed systems        |
| **HydraX**         | Proxy server       | —                                  |
| **Fast Server HD** | Proxy server       | —                                  |
| **PrimeVid**       | Self-hosted        | PrimeSrc's own video hosting       |
| **Enc-Dec.app**    | Proxy layer        | Used by Videasy, VidLink, LordFlix |

---

## 🛠️ Tools & WordPress Plugins

| Tool                     | For                       | URL                                                                           |
| ------------------------ | ------------------------- | ----------------------------------------------------------------------------- |
| **Dooplay Theme**        | WordPress streaming sites | [moviestreamingscripts.com](https://www.moviestreamingscripts.com)            |
| **PsyPlay Theme**        | WordPress streaming sites | [moviestreamingscripts.com](https://www.moviestreamingscripts.com)            |
| **DooPlay AutoEmbed**    | Integration plugin        | [superembed.stream](https://www.superembed.stream/dooplay.html)               |
| **Fmovies Theme 4.0.4**  | With VidSrc integration   | [Download](https://drive.google.com/file/d/1-Lsx9vEDvMW6WKVM8cZCW2sPGnMKVUwK) |
| **Latest Dooplay Theme** | With VidSrc integration   | [Download](https://drive.google.com)                                          |
| **Wovie Redux**          | Full theme + auto-embed   | [moviestreamingscripts.com](https://www.moviestreamingscripts.com)            |
| **ZetaFlix**             | Full streaming package    | [embed-api.stream](https://embed-api.stream/downloads/zetaflix1.zip)          |
| **FMovie PHP 7.4**       | Script package            | [embed-api.stream](https://embed-api.stream/downloads/fmovie74.zip)           |

---

## 🔑 Quick Reference — Embed Pattern

```html
<!-- Universal iframe embed pattern -->
<iframe
  src="https://PROVIDER_DOMAIN/..."
  width="100%"
  height="100%"
  frameborder="0"
  allowfullscreen
>
</iframe>
```

### ID Format Reference

| ID Type        | Format            | Example     | Source                                   |
| -------------- | ----------------- | ----------- | ---------------------------------------- |
| **IMDB ID**    | `tt` + 7-8 digits | `tt1375666` | [imdb.com](https://imdb.com)             |
| **TMDB ID**    | Numeric           | `27205`     | [themoviedb.org](https://themoviedb.org) |
| **AniList ID** | Numeric           | `21`        | [anilist.co](https://anilist.co)         |
| **TVMaze ID**  | Numeric           | `1234`      | [tvmaze.com](https://tvmaze.com)         |

---

## 📝 Notes

- Many embed servers **contain ads** (popups, banners) — they're free services.
- Availability changes frequently — domains get blocked and new ones appear.
- Most accept both **IMDB** (tt-prefixed) and **TMDB** (numeric) IDs.
- Always use **HTTPS** for embeds.
- Consider adding `allowfullscreen`, `allow="autoplay"` attributes to iframes.
- Some services require `&tmdb=1` flag when using TMDB IDs (e.g., 2embed,
  MultiEmbed).

---

> **Last updated:** July 2026  
> **Sources:** Official sites, GitHub repositories, community forums, direct
> inspection of embed players.

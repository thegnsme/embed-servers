# 🎬 Movie & TV Embed Servers — Complete Master List

> **12 parallel research agents · 50+ sources · Updated July 2026**
>
> Every server here accepts **TMDB ID** (numeric) or **IMDB ID** (tt-prefixed)
> unless noted. Format: `<iframe src="URL" ...>` embed pattern. 🔗 = hyperlinked
> working examples

---

## 📋 Table of Contents

1. [VidSrc Ecosystem (20+ domains)](#1-vidsrc-ecosystem)
2. [VidAPI / VaPlayer Network](#2-vidapi--vaplayer-network)
3. [2Embed Family](#3-2embed-family)
4. [SuperEmbed / MultiEmbed](#4-superembed--multiembed)
5. [VidCore](#5-vidcore)
6. [VidPlus (vidplus.to)](#6-vidplus)
7. [VidLux (vidlux.site)](#7-vidlux)
8. [Embed-API (embed-api.stream)](#8-embed-api)
9. [Vidify](#9-vidify)
10. [SmashyStream](#10-smashystream)
11. [PrimeSrc](#11-primesrc)
12. [VidPop](#12-vidpop)
13. [VikingEmbed / VEmbed](#13-vikingembed--vembed)
14. [EmbedMaster](#14-embedmaster)
15. [NontonGo](#15-nontongo)
16. [VIDEmbed (myflixerapi)](#16-vidembed-myflixerapi)
17. [AutoEmbed Network](#17-autoembed-network)
18. [VidLink](#18-vidlink)
19. [Videasy](#19-videasy)
20. [VidFast](#20-vidfast)
21. [VidRock](#21-vidrock)
22. [VidZee](#22-vidzee)
23. [VidNest](#23-vidnest)
24. [LordFlix](#24-lordflix)
25. [VixSrc](#25-vixsrc)
26. [CineSrc](#26-cinesrc)
27. [Peachify](#27-peachify)
28. [StreamMafia / NHD API](#28-streammafia--nhd-api)
29. [AnyEmbed](#29-anyembed)
30. [Other Embed Services (1Embed, CineSu, etc.)](#30-other-embed-services)
31. [Open Source / Self-Hosted APIs](#31-open-source--self-hosted-apis)
32. [Video Host Backends (file hosts)](#32-video-host-backends)
33. [Russian .ru / .su Embed Ecosystem](#33-russian-ru--su-embed-ecosystem)

---

## 1. VidSrc Ecosystem

**Official domain tracker:** [vidsrc.domains](https://vidsrc.domains/) ·
**Community:** [vidsrc.community](https://vidsrc.community/) · **Latest
announcement:** Switch to `vsembed.ru` / `vsembed.su`

### ✅ Currently Live (2026)

| #   | Domain                                     | Status           | Movie Endpoint         | TV Endpoint                 | Example                                             |
| --- | ------------------------------------------ | ---------------- | ---------------------- | --------------------------- | --------------------------------------------------- |
| 1   | [vsembed.ru](https://vsembed.ru)           | ✅ **Preferred** | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vsembed.ru/embed/movie/tt1375666)      |
| 2   | [vsembed.su](https://vsembed.su)           | ✅ **Preferred** | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vsembed.su/embed/movie/tt1375666)      |
| 3   | [vidsrcme.su](https://vidsrcme.su)         | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrcme.su/embed/movie/tt1375666)     |
| 4   | [vidsrc-me.ru](https://vidsrc-me.ru)       | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc-me.ru/embed/movie/tt1375666)    |
| 5   | [vidsrc-me.su](https://vidsrc-me.su)       | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc-me.su/embed/movie/tt1375666)    |
| 6   | [vidsrc-embed.ru](https://vidsrc-embed.ru) | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc-embed.ru/embed/movie/tt1375666) |
| 7   | [vidsrc-embed.su](https://vidsrc-embed.su) | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc-embed.su/embed/movie/tt1375666) |
| 8   | [vsrc.su](https://vsrc.su)                 | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vsrc.su/embed/movie/tt1375666)         |
| 9   | [vidsrc.fyi](https://vidsrc.fyi)           | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc.fyi/embed/movie/tt17048514)     |
| 10  | [vidsrc.wiki](https://vidsrc.wiki)         | ✅ Live          | `/embed/movie/{tmdb}`  | `/embed/tv/{tmdb}/{s}/{e}`  | [🔗](https://vidsrc.wiki/embed/movie/533535)        |
| 11  | [vidsrc.to](https://vidsrc.to)             | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc.to/embed/movie/tt1375666)       |
| 12  | [vidsrc.cc](https://vidsrc.cc)             | ✅ Live          | `/v2/embed/movie/{id}` | `/v2/embed/tv/{id}/{s}/{e}` | [🔗](https://vidsrc.cc/v2/embed/movie/tt1375666)    |
| 13  | [vidsrc.io](https://vidsrc.io)             | ⚠️ Old           | `/embed/{id}`          | `/embed/{id}/{s}-{e}`       | [🔗](https://vidsrc.io/embed/tt1375666)             |
| 14  | [vidsrc.bz](https://vidsrc.bz)             | ⚠️ Old           | `/embed/{id}`          | `/embed/{id}/{s}-{e}`       | [🔗](https://vidsrc.bz/embed/tt1375666)             |
| 15  | [vidsrc.do](https://vidsrc.do)             | ⚠️ Old           | `/embed/{id}`          | `/embed/{id}/{s}-{e}`       | [🔗](https://vidsrc.do/embed/tt1375666)             |
| 16  | [vidsrc.tw](https://vidsrc.tw)             | ⚠️ Old           | `/embed/{id}`          | `/embed/{id}/{s}-{e}`       | [🔗](https://vidsrc.tw/embed/tt1375666)             |
| 17  | [vidsrc.sbs](https://vidsrc.sbs)           | ✅ Live          | `/embed/movie/{tmdb}`  | `/embed/tv/{tmdb}/{s}/{e}`  | [🔗](https://vidsrc.sbs/embed/movie/533535)         |
| 18  | [vidsrc.mov](https://vidsrc.mov)           | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc.mov/embed/movie/tt1375666)      |
| 19  | [vidsrc.online](https://vidsrc.online)     | ✅ Live          | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc.online/embed/movie/tt1375666)   |
| 20  | [vidsrc.icu](https://vidsrc.icu)           | ⚠️ Unknown       | `/embed/movie/{id}`    | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://vidsrc.icu/embed/movie/tt1375666)      |

### ❌ Dead VidSrc Domains

`vidsrc.in` · `vidsrc.net` · `vidsrc.xyz` · `vidsrc.pm` · `vidsrc.vc` ·
`vidsrc.mn` · `vidsrc.gd` · `vidsrc.me` · `vidsrc.pro`

### 📐 VidSrc Extra API Endpoints

```
Latest movies:  GET /vapi/movie/new/{page}
Latest adds:    GET /vapi/movie/add/{page}
Latest TV:      GET /vapi/tv/new/{page}
Episodes feed:  GET /vapi/episode/latest
Subs:           ?sub.info=[{"file":"URL","label":"LANG"}]
Custom color:   See v2.vidsrc.me/embed/{id}/color-{hex}
Lists (v2):     GET /movies/latest/page-{N}.json
Lists (v2):     GET /episodes/latest/page-{N}.json
```

---

## 2. VidAPI / VaPlayer Network

**Domain tracker:** [vidapi.domains](https://vidapi.domains/)

| #   | Domain                             | Status        | Movie Endpoint      | TV Endpoint              | Example                                         |
| --- | ---------------------------------- | ------------- | ------------------- | ------------------------ | ----------------------------------------------- |
| 1   | [vidapi.to](https://vidapi.to)     | ✅ Portal     | `-> vaplayer.ru`    | —                        | Portal                                          |
| 2   | [vidapi.me](https://vidapi.me)     | ✅ Portal     | `-> vaplayer.ru`    | —                        | Portal                                          |
| 3   | [vidapi.bz](https://vidapi.bz)     | ✅ Portal     | `-> vaplayer.ru`    | —                        | Portal                                          |
| 4   | [vidapi.tw](https://vidapi.tw)     | ✅ Portal     | `-> vaplayer.ru`    | —                        | Portal                                          |
| 5   | [vidapi.ru](https://vidapi.ru)     | ❌ Dead       | —                   | —                        | —                                               |
| 6   | [vidapi.xyz](https://vidapi.xyz)   | ✅ Live       | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}` | [🔗](https://vidapi.xyz/embed/movie/tt1375666)  |
| 7   | [vaplayer.ru](https://vaplayer.ru) | ✅ **Player** | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}` | [🔗](https://vaplayer.ru/embed/movie/tt1375666) |

---

## 3. 2Embed Family

| #   | Domain                                     | Status  | Movie Endpoint      | TV Endpoint                 | Example                                               |
| --- | ------------------------------------------ | ------- | ------------------- | --------------------------- | ----------------------------------------------------- |
| 1   | [2embed.cc](https://www.2embed.cc)         | ✅ Live | `/embed/{id}`       | `/embedtv/{id}&s={n}&e={n}` | [🔗](https://www.2embed.cc/embed/tt1375666)           |
| 2   | [2embed.skin](https://2embed.skin)         | ✅ Live | `/embed/{id}`       | `/embedtv/{id}&s={n}&e={n}` | [🔗](https://2embed.skin/embed/tt1375666)             |
| 3   | [2embed.top](https://2embed.top)           | ✅ Live | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://2embed.top/embed/movie/tt1375666)        |
| 4   | [2embed.stream](https://2embed.stream)     | ✅ Live | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://2embed.stream/embed/movie/tt1375666)     |
| 5   | [2embed.online](https://www.2embed.online) | ✅ Live | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://www.2embed.online/embed/movie/tt1375666) |
| 6   | [hnembed.cc](https://hnembed.cc)           | ✅ Live | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://hnembed.cc/embed/movie/tt1375666)        |
| 7   | [hnembed.com](https://hnembed.com)         | ✅ Live | `/embed/movie/{id}` | `/embed/tv/{id}/{s}/{e}`    | [🔗](https://hnembed.com/embed/movie/tt1375666)       |

**JSON API:** `https://api.2embed.cc/movie?imdb_id={tt...}` ·
`https://api.2embed.cc/tv?imdb_id={tt...}`

---

## 4. SuperEmbed / MultiEmbed

**Website:** [superembed.stream](https://www.superembed.stream/)

| Endpoint         | URL                                                                 | Example                                                                  |
| ---------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| **Movie (IMDB)** | `https://multiembed.mov/?video_id={imdb}`                           | [🔗](https://multiembed.mov/?video_id=tt1375666)                         |
| **Movie (TMDB)** | `https://multiembed.mov/?video_id={tmdb}&tmdb=1`                    | [🔗](https://multiembed.mov/?video_id=27205&tmdb=1)                      |
| **TV (IMDB)**    | `https://multiembed.mov/?video_id={imdb}&s={n}&e={n}`               | [🔗](https://multiembed.mov/?video_id=tt0944947&s=1&e=1)                 |
| **TV (TMDB)**    | `https://multiembed.mov/?video_id={tmdb}&tmdb=1&s={n}&e={n}`        | [🔗](https://multiembed.mov/?video_id=1399&tmdb=1&s=1&e=1)               |
| **VIP Movie**    | `https://multiembed.mov/directstream.php?video_id={id}`             | [🔗](https://multiembed.mov/directstream.php?video_id=tt1375666)         |
| **VIP TV**       | `https://multiembed.mov/directstream.php?video_id={id}&s={n}&e={n}` | [🔗](https://multiembed.mov/directstream.php?video_id=tt0944947&s=1&e=1) |
| **VIP Check**    | Add `&check=1`                                                      | Returns 0 or 1                                                           |
| **Custom subs**  | `&sub_url={url}&sub_label={label}`                                  |                                                                          |

**JSON API:** `https://seapi.link/?type=imdb&id={id}` ·
`https://seapi.link/?type=tmdb&id={id}` ·
`https://seapi.link/?type=search&query={title}`

---

## 5. VidCore

**Website:** [vidcore.org](https://www.vidcore.org/) · **Docs:**
[vidcore.org](https://www.vidcore.org/)

| Type      | Endpoint                                      | Example                                     |
| --------- | --------------------------------------------- | ------------------------------------------- |
| **Movie** | `https://vidcore.org/embed/movie/{tmdb}`      | [🔗](https://vidcore.org/embed/movie/27205) |
| **TV**    | `https://vidcore.org/embed/tv/{tmdb}/{s}/{e}` | [🔗](https://vidcore.org/embed/tv/1399/1/1) |

**Params:** `autoPlay`, `startAt`, `theme` (hex), `server`, `hideServer`, `sub`,
`chromecast`, `poster`, `title`, `fullscreenButton`

**Alt domain:** [vidcore.created.app](https://vidcore.created.app)

---

## 6. VidPlus

**Website:** [vidplus.to](https://vidplus.to) · **GitHub:**
[vidbox1/vidplus](https://github.com/vidbox1/vidplus)

| Type      | Endpoint                                                      | Example                                            |
| --------- | ------------------------------------------------------------- | -------------------------------------------------- |
| **Movie** | `https://player.vidplus.to/embed/movie/{tmdb}`                | [🔗](https://player.vidplus.to/embed/movie/27205)  |
| **TV**    | `https://player.vidplus.to/embed/tv/{tmdb}/{s}/{e}`           | [🔗](https://player.vidplus.to/embed/tv/94997/1/1) |
| **Anime** | `https://player.vidplus.to/embed/anime/{anilistId}/{ep}?dub=` | [🔗](https://player.vidplus.to/embed/anime/21/1)   |

**Params:** `autoplay`, `autonext`, `nextbutton`, `progress`, `primarycolor`,
`secondarycolor`, `iconcolor`, `poster`, `title`, `chromecast`, `server`,
`watchparty`, `font`, `fontcolor`, `fontsize`, `opacity`, `logourl`, `icons`,
`hideposter`, `hidetitle`, `hidechromecast`, `hidepip`, `hideepisodelist`,
`hideservericon`

---

## 7. VidLux

**Website:** [vidlux.site](https://vidlux.site) · **GitHub:**
[segseaweber/vidlux-streaming-api](https://github.com/segseaweber/vidlux-streaming-api)
· **Requires API key**

| Type      | Endpoint                                                | Example                                               |
| --------- | ------------------------------------------------------- | ----------------------------------------------------- |
| **Movie** | `https://vidlux.site/embed/movie/{tmdb}?key={key}`      | [🔗](https://vidlux.site/embed/movie/603692?key=demo) |
| **TV**    | `https://vidlux.site/embed/tv/{tmdb}/{s}/{e}?key={key}` | [🔗](https://vidlux.site/embed/tv/1399/1/1?key=demo)  |

**Servers:** Alpha, Nova, Astra, Flix, Delta, Omega

**Alt domains:** `vidlux.xyz` · `vidlux.top` · `vidlux.online`

---

## 8. Embed-API

**Website:** [embed-api.stream](https://embed-api.stream) · **Player:**
[player.embed-api.stream](https://player.embed-api.stream)

| Type      | Endpoint                                                 | Example                                                 |
| --------- | -------------------------------------------------------- | ------------------------------------------------------- |
| **Movie** | `https://player.embed-api.stream/?id={tmdb}`             | [🔗](https://player.embed-api.stream/?id=786892)        |
| **TV**    | `https://player.embed-api.stream/?id={tmdb}&s={n}&e={n}` | [🔗](https://player.embed-api.stream/?id=76479&s=4&e=1) |

**Aggregates:** MoviesAPI, VidZee, Vidify, VidRock, MappleTV, VidLink,
PrimeWire, MultiEmbed, VidBinge, VidSrc, AutoEmbed, 2Embed

---

## 9. Vidify

**Player:** [player.vidify.top](https://player.vidify.top)

| Type      | Endpoint                                            | Example                                           |
| --------- | --------------------------------------------------- | ------------------------------------------------- |
| **Movie** | `https://player.vidify.top/embed/movie/{tmdb}`      | [🔗](https://player.vidify.top/embed/movie/27205) |
| **TV**    | `https://player.vidify.top/embed/tv/{tmdb}/{s}/{e}` | [🔗](https://player.vidify.top/embed/tv/1399/1/1) |

**Params:** `primaryColor`, `secondaryColor`, `iconColor`, `autoplay`, `poster`,
`server`, `font`, `fontcolor`, `fontsize`, `opacity`, `logourl`, `pip`,
`chromecast`

---

## 10. SmashyStream

**Player:** [player.smashy.stream](https://player.smashy.stream)

| Type      | Endpoint                                           | Example                                                 |
| --------- | -------------------------------------------------- | ------------------------------------------------------- |
| **Movie** | `https://player.smashy.stream/movie/{id}`          | [🔗](https://player.smashy.stream/movie/tt4154796)      |
| **TV**    | `https://player.smashy.stream/tv/{id}?s={n}&e={n}` | [🔗](https://player.smashy.stream/tv/tt0903747?s=1&e=5) |

**Params:** `btPosition`, `playerList`, `remove`, `startTime`, `subLang`

---

## 11. PrimeSrc

**Website:** [primesrc.me](https://primesrc.me) · **Library:** 77K+ movies,
275K+ episodes

| Type             | Endpoint                                                          | Example                                                          |
| ---------------- | ----------------------------------------------------------------- | ---------------------------------------------------------------- |
| **Movie (IMDB)** | `https://primesrc.me/embed/movie?imdb={id}`                       | [🔗](https://primesrc.me/embed/movie?imdb=tt0848228)             |
| **Movie (TMDB)** | `https://primesrc.me/embed/movie?tmdb={id}`                       | [🔗](https://primesrc.me/embed/movie?tmdb=24428)                 |
| **TV (TMDB)**    | `https://primesrc.me/embed/tv?tmdb={id}&season={n}&episode={n}`   | [🔗](https://primesrc.me/embed/tv?tmdb=32726&season=1&episode=1) |
| **TV (TVMaze)**  | `https://primesrc.me/embed/tv?tvmaze={id}&season={n}&episode={n}` |                                                                  |

**JSON API:** `https://primesrc.me/api/v1/list_servers?type=movie&imdb={id}`

Aggregates **14+ file hosting servers**. Built with Elixir/Phoenix + Cloudflare.

---

## 12. VidPop

**Website:** [vidpop.xyz](https://vidpop.xyz)

| Type      | Endpoint                                                         | Example                                                        |
| --------- | ---------------------------------------------------------------- | -------------------------------------------------------------- |
| **Movie** | `https://www.vidpop.xyz/embed/?id={tmdb}`                        | [🔗](https://www.vidpop.xyz/embed/?id=27205)                   |
| **TV**    | `https://www.vidpop.xyz/embed/?id={tmdb}&season={n}&episode={n}` | [🔗](https://www.vidpop.xyz/embed/?id=1399&season=1&episode=1) |

---

## 13. VikingEmbed / VEmbed

**Website:** [vembed.stream](https://vembed.stream)

| Type         | Endpoint                                      | Example                                    |
| ------------ | --------------------------------------------- | ------------------------------------------ |
| **Movie/TV** | `https://vembed.stream/play/{id}`             | [🔗](https://vembed.stream/play/tt1375666) |
| **Season**   | `https://vembed.stream/play/{tmdb}_s{season}` |                                            |

**Telegram:** [t.me/vikingembed](https://t.me/vikingembed)

---

## 14. EmbedMaster

**Website:** [embedmaster.com](https://embedmaster.com) · **Docs:**
[embedmaster.com/documentation](https://embedmaster.com/documentation/)

| Type            | Endpoint                                   | Example                                         |
| --------------- | ------------------------------------------ | ----------------------------------------------- |
| **Movie**       | `https://embedmaster.link/movie/{id}`      | [🔗](https://embedmaster.link/movie/tt1375666)  |
| **TV**          | `https://embedmaster.link/tv/{id}/{s}/{e}` | [🔗](https://embedmaster.link/tv/tt0944947/1/1) |
| **Custom subs** | `?sub_url[]={url}&sub_label[]={label}`     |                                                 |

Requires registration. 10+ premium servers (StreamTape, DoodStream, FlixHQ,
etc.). Ad-free option.

---

## 15. NontonGo

**Website:** [nontongo.win](https://www.nontongo.win)

| Type             | Endpoint                                                 | Example                                                    |
| ---------------- | -------------------------------------------------------- | ---------------------------------------------------------- |
| **Movie (IMDB)** | `https://www.nontongo.win/embed/movie/{imdb}`            | [🔗](https://www.nontongo.win/embed/movie/tt1375666)       |
| **Movie (TMDB)** | `https://www.nontongo.win/embed/movie/{tmdb}`            | [🔗](https://www.nontongo.win/embed/movie/27205)           |
| **TV**           | `https://www.nontongo.win/embed/tv/{id}/{s}/{e}`         | [🔗](https://www.nontongo.win/embed/tv/tt0944947/1/1)      |
| **TV (alt)**     | `https://www.nontongo.win/embed/tv/?id={id}&s={n}&e={n}` |                                                            |
| **Anime**        | `https://nontongo.win/embed/anime/{slug}`                | [🔗](https://nontongo.win/embed/anime/one-piece-episode-1) |

---

## 16. VIDEmbed (myflixerapi)

**Website:** [vidsrc.myflixerapi.com](https://vidsrc.myflixerapi.com/api) ·
**Rate limit:** 100/day

| Type              | Endpoint                                                                |
| ----------------- | ----------------------------------------------------------------------- |
| **Movie (IMDB)**  | `https://vidsrc.myflixerapi.com/embed/movie?imdb={id}`                  |
| **Movie (TMDB)**  | `https://vidsrc.myflixerapi.com/embed/movie?tmdb={id}`                  |
| **Movie (title)** | `https://vidsrc.myflixerapi.com/embed/movie?title={t}&year={y}`         |
| **TV (IMDB)**     | `https://vidsrc.myflixerapi.com/embed/series?imdb={id}&sea={s}&epi={e}` |
| **TV (TMDB)**     | `https://vidsrc.myflixerapi.com/embed/series?tmdb={id}&sea={s}&epi={e}` |
| **TV (path)**     | `https://vidsrc.myflixerapi.com/embed/{showId}/{s}/{e}`                 |
| **Download**      | Replace `embed` → `download` in any URL                                 |
| **Status**        | `https://vidsrc.myflixerapi.com/api/status?imdb={id}&type=movie`        |

---

## 17. AutoEmbed Network

| Domain                                                 | Type   | Endpoint                  |
| ------------------------------------------------------ | ------ | ------------------------- |
| [player.autoembed.app](https://player.autoembed.app)   | Movie  | `/embed/movie/{id}`       |
|                                                        | TV     | `/embed/tv/{id}/{s}/{e}`  |
| [autoembed.co](https://autoembed.co)                   | Movie  | `/movie/tmdb/{tmdb}`      |
|                                                        | TV     | `/tv/tmdb/{tmdb}-{s}-{e}` |
| [autoembed.cc](https://autoembed.cc)                   | Movie  | `/embed/movie/{id}`       |
|                                                        | TV     | `/embed/tv/{id}/{s}/{e}`  |
| [watch-v2.autoembed.cc](https://watch-v2.autoembed.cc) | Movie  | `/movie/{tmdb}`           |
|                                                        | TV     | `/tv/{tmdb}`              |
| [autoembed.net](https://autoembed.net)                 | Portal | Discord community         |

---

## 18. VidLink

**Website:** [vidlink.pro](https://vidlink.pro)

| Type      | Endpoint                                            | Example                               |
| --------- | --------------------------------------------------- | ------------------------------------- |
| **Movie** | `https://vidlink.pro/movie/{tmdb}`                  | [🔗](https://vidlink.pro/movie/27205) |
| **TV**    | `https://vidlink.pro/tv/{tmdb}/{s}/{e}`             | [🔗](https://vidlink.pro/tv/1399/1/1) |
| **Anime** | `https://vidlink.pro/anime/{malId}/{ep}/{sub\|dub}` |                                       |

Uses WASM encryption. Also accessible via `enc-dec.app` proxy.

---

## 19. Videasy

**Website:** [player.videasy.net](https://player.videasy.net) · **Alt domain:**
[vidking.net](https://www.vidking.net)

| Type      | Endpoint                                       | Example                                      |
| --------- | ---------------------------------------------- | -------------------------------------------- |
| **Movie** | `https://player.videasy.net/movie/{tmdb}`      | [🔗](https://player.videasy.net/movie/27205) |
| **TV**    | `https://player.videasy.net/tv/{tmdb}/{s}/{e}` | [🔗](https://player.videasy.net/tv/1399/1/1) |

**Servers (10):** Neon, Yoru, Cypher, Reyna, Omen, Breach, Ghost, Sage, Vyse,
Raze

**API:**
`https://api.videasy.net/{server}/sources-with-title?title={t}&mediaType={type}&year={y}&tmdbId={id}&imdbId={id}`

---

## 20. VidFast

**Domains:** [vidfast.pro](https://vidfast.pro) ·
[vidfast.vc](https://vidfast.vc) · [vidfast.pm](https://vidfast.pm)

| Type      | Endpoint                                            | Example                               |
| --------- | --------------------------------------------------- | ------------------------------------- |
| **Movie** | `https://vidfast.pro/movie/{id}?autoPlay=true`      | [🔗](https://vidfast.pro/movie/27205) |
| **TV**    | `https://vidfast.pro/tv/{id}/{s}/{e}?autoPlay=true` | [🔗](https://vidfast.pro/tv/1399/1/1) |

---

## 21. VidRock

**Domain:** [vidrock.net](https://vidrock.net) · **API:** `sub.vdrk.site` ·
`proxy.vidrock.store`

| Type      | Endpoint                                                          | Example                               |
| --------- | ----------------------------------------------------------------- | ------------------------------------- |
| **Movie** | `https://vidrock.net/movie/{id}?autoplay=true`                    | [🔗](https://vidrock.net/movie/27205) |
| **TV**    | `https://vidrock.net/tv/{id}/{s}/{e}?autoplay=true&autonext=true` | [🔗](https://vidrock.net/tv/1399/1/1) |

---

## 22. VidZee

**Domain:** [player.vidzee.wtf](https://player.vidzee.wtf) · **API:**
`core.vidzee.wtf`

| Type      | Endpoint                                            | Example                                           |
| --------- | --------------------------------------------------- | ------------------------------------------------- |
| **Movie** | `https://player.vidzee.wtf/embed/movie/{tmdb}`      | [🔗](https://player.vidzee.wtf/embed/movie/27205) |
| **TV**    | `https://player.vidzee.wtf/embed/tv/{tmdb}/{s}/{e}` | [🔗](https://player.vidzee.wtf/embed/tv/1399/1/1) |

---

## 23. VidNest

**Domain:** [vidnest.fun](https://vidnest.fun) · **Alt:** `new.vidnest.fun`

| Type      | Endpoint                                            | Example                               |
| --------- | --------------------------------------------------- | ------------------------------------- |
| **Movie** | `https://vidnest.fun/movie/{tmdb}`                  | [🔗](https://vidnest.fun/movie/27205) |
| **TV**    | `https://vidnest.fun/tv/{tmdb}/{s}/{e}`             | [🔗](https://vidnest.fun/tv/1399/1/1) |
| **Anime** | `https://vidnest.fun/anime/{anilistId}/{ep}/{lang}` |                                       |

**Servers:** moviebox, allmovies, catflix, purstream, hollymoviehd, lamda,
flixhq, vidlink, onehd, klikxxi

---

## 24. LordFlix

**Domains:** [lordflix.org](https://lordflix.org) · `snowhouse.lordflix.club`

**Endpoint:**
`snowhouse.lordflix.club/?title={t}&type={type}&year={y}&imdb={id}&tmdb={id}&server={server}`

**Servers (9):** Berlin, Marseille, Backrooms, Phoenix, Oslo, Luna, Sakura, Rio,
Ativa, Moscow

---

## 25. VixSrc

**Domain:** [vixsrc.to](https://vixsrc.to)

| Type      | Endpoint                                  | Example                                 |
| --------- | ----------------------------------------- | --------------------------------------- |
| **Movie** | `https://vixsrc.to/api/movie/{tmdb}`      | [🔗](https://vixsrc.to/api/movie/27205) |
| **TV**    | `https://vixsrc.to/api/tv/{tmdb}/{s}/{e}` | [🔗](https://vixsrc.to/api/tv/1399/1/1) |

---

## 26. CineSrc

**Domain:** [cinesrc.st](https://cinesrc.st)

| Type           | Endpoint                                     |
| -------------- | -------------------------------------------- |
| **Movie**      | `https://cinesrc.st/embed/movie/{tmdb}`      |
| **TV**         | `https://cinesrc.st/embed/tv/{tmdb}/{s}/{e}` |
| **Stream API** | `/api/stream/live?id={id}&type=movie` (SSE)  |
| **Proxy**      | `/api/proxy?url={streamUrl}` (HLS relay)     |

---

## 27. Peachify

**Domains:** [peachify.top](https://peachify.top) · `uwu.eat-peach.sbs` ·
`usa.eat-peach.sbs`

**Servers:** moviebox, holly, air, multi, net, bmb

---

## 28. StreamMafia / NHD API

**Domain:** `player.nhdapi.com`

| Type        | Endpoint                  |
| ----------- | ------------------------- |
| **Movie**   | `/api/movie/{tmdb}`       |
| **TV**      | `/api/tv/{tmdb}/{s}/{e}`  |
| **Source**  | `/api/source/{file_code}` |
| **Token**   | `/api/token`              |
| **Session** | `/api/session`            |

---

## 29. AnyEmbed

**Domain:** [anyembed.xyz](https://anyembed.xyz) · **API:** `api.anyembed.xyz`

| Type        | Endpoint                                        |
| ----------- | ----------------------------------------------- |
| **Stream**  | `https://api.anyembed.xyz/api/v1/stream/{tmdb}` |
| **Session** | `https://api.anyembed.xyz/api/v1/session`       |

---

## 30. Other Embed Services

| #   | Domain                                         | Movie Endpoint                      | TV Endpoint                                      |
| --- | ---------------------------------------------- | ----------------------------------- | ------------------------------------------------ |
| 1   | [1embed.cc](https://1embed.cc)                 | `/embed/movie/{tmdb}`               | `/embed/tv/{id}/{s}/{e}`                         |
| 2   | [vidsync.xyz](https://vidsync.xyz)             | `/embed/movie/{id}?autoPlay=true`   | `/embed/tv/{id}/{s}/{e}`                         |
| 3   | [vidsrc.rip](https://vidsrc.rip)               | `/embed/movie/{id}`                 | `/embed/tv/{id}/{s}/{e}`                         |
| 4   | [flixer.su](https://flixer.su)                 | `/watch/movie/{tmdb}`               | `/watch/tv/{tmdb}/{s}/{e}`                       |
| 5   | [hexa.watch](https://hexa.watch)               | `/watch/movie/{id}`                 | `/watch/tv/{id}/{s}/{e}`                         |
| 6   | [vidjoy.pro](https://vidjoy.pro)               | `/embed/movie/{id}`                 | `/embed/tv/{id}/{s}/{e}`                         |
| 7   | [rivestream.app](https://rivestream.app)       | `/embed?type=movie&id={id}`         | `/embed?type=tv&id={id}&season={n}&episode={n}`  |
| 8   | [wavembed.lol](https://wavembed.lol)           | `/movie/{tmdb}?api={0-7}`           | `/tv/{tmdb}/{s}/{e}?api={0-7}`                   |
| 9   | [anyplay.stream](https://www.anyplay.stream)   | `/embed/movie/{serverId}/{tmdb}`    | `/embed/movie/{serverId}/{tmdb}/{s}/{e}`         |
| 10  | [streamflix.one](https://streamflix.one)       | `/movie/{id}?server=1`              | `/tv/{id}/watch?server=1&season={n}&episode={n}` |
| 11  | [nebulaflix.stream](https://nebulaflix.stream) | `/movie?mt={id}&server=1`           | `/show?st={id}&season={n}&episode={n}&server=1`  |
| 12  | [videasy.net](https://videasy.net)             | `/movie/{id}?color=`                | `/tv/{id}/{s}/{e}?color=`                        |
| 13  | [frembed.com](https://frembed.com)             | `/api/film.php?id={id}`             | `/api/serie.php?id={id}&sa={n}&epi={n}`          |
| 14  | [embed.su](https://embed.su)                   | `/embed/movie/{id}`                 | `/embed/tv/{id}/{s}/{e}`                         |
| 15  | [embedbandit.com](http://embedbandit.com)      | `/embed/movie?tmdb={id}`            | `/embed/tv?tmdb={id}&season={n}&episode={n}`     |
| 16  | [111movies.com](https://111movies.com)         | `/movie/{id}`                       | `/tv/{id}/{s}/{e}`                               |
| 17  | [moviesapi.to](https://moviesapi.to)           | `/movie/{id}`                       | `/tv/{id}-{s}-{e}`                               |
| 18  | [spencerdevs.xyz](https://spencerdevs.xyz)     | `/movie/{tmdb}`                     | `/tv/{tmdb}/{s}/{e}`                             |
| 19  | [ezvidapi.com](https://ezvidapi.com)           | `/embed/movie/{tmdb}`               | `/embed/tv/{tmdb}/{s}/{e}`                       |
| 20  | [cine.su](https://cine.su)                     | `/v1/stream/master/movie/{id}.m3u8` | `/v1/stream/master/tv/{id}/{s}/{e}.m3u8`         |
| 21  | [icefy.top](https://streams.icefy.top)         | `/movie/{id}`                       | `/tv/{id}/{s}/{e}`                               |
| 22  | [fsharetv.cc](https://fsharetv.cc)             | `/movie/{imdb}`                     |                                                  |
| 23  | [netoda.tech](https://netoda.tech)             | Embed service                       |                                                  |
| 24  | [uembed.xyz](https://uembed.xyz)               | Embed service                       |                                                  |
| 25  | [cloudnestra.com](https://cloudnestra.com)     | CDN/player domain                   |                                                  |

### 🌐 vidembed.site Family

| Domain                                 | Endpoint            |
| -------------------------------------- | ------------------- |
| [vidembed.site](https://vidembed.site) | `/embed/movie/{id}` |
| [vidembed.su](https://vidembed.su)     | `/embed/movie/{id}` |
| [megaembed.cc](https://megaembed.cc)   | `/embed/movie/{id}` |
| [megaembed.su](https://megaembed.su)   | `/embed/movie/{id}` |
| [vidstorm.ru](https://vidstorm.ru)     | `/embed/movie/{id}` |
| [vidstorm.su](https://vidstorm.su)     | `/embed/movie/{id}` |

### 🌐 StreamVault

| Type       | Endpoint                   |
| ---------- | -------------------------- |
| **Domain** | `streamvaultsrc.click`     |
| **Movie**  | `/embed/movie/{tmdb}`      |
| **TV**     | `/embed/tv/{tmdb}/{s}/{e}` |

**Params:** `autoplay`, `muted`, `seek`, `quality`, `autonext`, `back`

### 🌐 NexStream (CodeSpecter)

**Domain:** `api.codespecters.com` · **Requires API key (free)**

| Type      | Endpoint                                |
| --------- | --------------------------------------- |
| **Movie** | `/embed/movie/{tmdb}?apikey={key}`      |
| **TV**    | `/embed/tv/{tmdb}/{s}/{e}?apikey={key}` |

### 🌐 Legacy / Down Services

| Domain                                     | Endpoint                                          | Status            |
| ------------------------------------------ | ------------------------------------------------- | ----------------- |
| [fsapi.xyz](https://fsapi.xyz)             | `/movie/{imdb}` / `/tv-imdb/{id}-{s}-{e}`         | ⚠️ Likely dead    |
| [moviewp.com](https://moviewp.com)         | `/se.php?video_id={id}`                           | ❌ API dead       |
| [curtstream.com](https://curtstream.com)   | `/movies/imdb/{id}` / `/series/tmdb/{id}/{s}/{e}` | ❌ Domain expired |
| [vplus.ucoz.com](https://vplus.ucoz.com)   | `/{imdbId}`                                       | ⚠️ Old, limited   |
| [hydramovies.com](https://hydramovies.com) | `/api-v2/?imdb_id={id}`                           | ⚠️ CSV data only  |

---

## 31. Open Source / Self-Hosted APIs

### TMDB Embed API

**GitHub:**
[Inside4ndroid/TMDB-Embed-API](https://github.com/Inside4ndroid/TMDB-Embed-API)
⭐121 · MIT · Docker ready

**Built-in providers:** Showbox, 4KHDHub, VixSrc, Videasy, VidLink, LordFlix,
NoTorrent, DahmerMovies

```
GET /api/streams/movie/{tmdbId}
GET /api/streams/tv/{tmdbId}?season={n}&episode={n}
GET /api/streams/{provider}/{type}/{tmdbId}
GET /api/providers
GET /api/health
```

### CinePro Backend

**GitHub:** [cinepro-org/backend](https://github.com/cinepro-org/backend) ⭐125

**Providers:** VidSrc, VidSrcCC, MultiEmbed, AutoEmbed, Xprime, PrimeWire

```
GET /movie/{tmdbId}
GET /tv/{tmdbId}?s={season}&e={episode}
```

### CinePro Core (successor)

**GitHub:** [cinepro-org/core](https://github.com/cinepro-org/core) ·
OMSS-compliant · **50+ sources**

**Providers:** vidsrc, vixsrc, vidapi, vidzee, vidnest, vidrock, cinesu, icefy,
fsharetv, peachify, streammafia, tulnex, anyembed, videasy, fmovies4u, popr,
02moviedownloader

### VidSrc Scraper

**GitHub:**
[DivineChile/vidsrc-scraper](https://github.com/DivineChile/vidsrc-scraper) ·
Node.js + Playwright

### Consumet API

**Website:** [docs.consumet.org](https://docs.consumet.org) · **API:**
[api.consumet.org](https://api.consumet.org)

**Providers:** FlixHQ, Goku, HiMovies, SFlix, MovieHdWatch, ViewAsian

### Enc-Dec Endpoints

**GitHub:** [smy778/EncDecEndpoints](https://github.com/smy778/EncDecEndpoints)
⭐64

Central encryption proxy supporting: AnimeKai, YFlix, VidLink, VidSync, Videasy,
VidFast, VidCore, VidUp, LordFlix, Peachify, CineSrc, Hexa, Flixer, KissKH,
MeowTV, OneTouchTV, MegaUp, RapidShare, Abyss, FlixCloud

---

## 32. Video Host Backends

Underlying file hosts that the embed servers aggregate from:

| Host           | URL                                      | Used By                       |
| -------------- | ---------------------------------------- | ----------------------------- |
| **StreamTape** | [streamtape.com](https://streamtape.com) | SuperEmbed, EmbedMaster, many |
| **DoodStream** | [doodstream.com](https://doodstream.com) | SuperEmbed, EmbedMaster, many |
| **MixDrop**    | [mixdrop.co](https://mixdrop.co)         | SuperEmbed, many              |
| **FileMoon**   | [filemoon.org](https://filemoon.org)     | EmbedMaster, many             |
| **VidMoly**    | [vidmoly.me](https://vidmoly.me)         | EmbedMaster                   |
| **VOE**        | [voe.sx](https://voe.sx)                 | SuperEmbed, EmbedMaster       |
| **StreamSB**   | [streamsb.net](https://streamsb.net)     | SuperEmbed                    |
| **UpStream**   | [upstream.to](https://upstream.to)       | SuperEmbed                    |
| **Abyss**      | [abyss.to](https://abyss.to)             | SuperEmbed, Enc-Dec           |
| **StreamHide** | [streamhide.to](https://streamhide.to)   | SuperEmbed                    |
| **BigWarp**    | [bigwarp.io](https://bigwarp.io)         | EmbedMaster                   |
| **EarnVids**   | earnvids.com                             | EmbedMaster                   |
| **SaveFiles**  | savefiles.com                            | EmbedMaster                   |
| **StreamWish** | [streamwish.to](https://streamwish.to)   | EmbedMaster                   |
| **FlixHQ**     | flixhq.co                                | EmbedMaster, Consumet         |
| **VidPlay**    | vidplay.com                              | VidSrc network                |
| **HydraX**     | playhydrax.com                           | Older embed systems           |
| **GDrive**     | —                                        | Google Drive proxy            |
| **PrimeVid**   | —                                        | PrimeSrc self-hosted          |
| **Showbox**    | febbox.com                               | TMDB-Embed-API                |
| **NoTorrent**  | addon-osvh.onrender.com                  | Stremio addon API             |

### 4KHDHub File Host Sources (35+)

From `phisher98/TVVVV/domains.json`: `moviesdrives.my` · `hdhub4u.cl` ·
`multimovies.makeup` · `bollyflix.at` · `uhdmovies.casa` · `moviesmod.army` ·
`vegamovies.navy` · `rogmovies.rest` · `luxmovies1.shop` · `123moviesfree9.cv` ·
`extramovies.miami` · `banglaplex.lat` · `telugumv.net` · `filmycab.co` ·
`tellyhd.im` · `filmyfly.cafe` · `hindmovie.icu` · `1tamilblasters.pro` ·
`hubcloud.cx` · `movienestbd.pics` · `movies4u.clinic` · `cinevoodc.com` ·
`dudefilms.living` · `fibwatch.art` · `fibtoon.top` · `fibdrama.top` ·
`xprimehub.bond` · `m4ufree.lat` · `zinkmovies.today` · `cinefreak.nl` ·
`pixeldrain.dev`

---

## 33. Russian .ru / .su Embed Ecosystem

A significant portion of embed servers now operate under Russian (.ru) and
Soviet (.su) TLDs:

| Domain          | TLD | Service                  |
| --------------- | --- | ------------------------ |
| vsembed.ru      | .ru | VidSrc **new preferred** |
| vsembed.su      | .su | VidSrc **new preferred** |
| vidsrc-embed.ru | .ru | VidSrc embed             |
| vidsrc-embed.su | .su | VidSrc embed             |
| vidsrcme.ru     | .ru | VidSrc portal            |
| vidsrcme.su     | .su | VidSrc portal            |
| vidsrc-me.ru    | .ru | VidSrc portal            |
| vidsrc-me.su    | .su | VidSrc portal            |
| vsrc.su         | .su | VidSrc short domain      |
| vidapi.ru       | .ru | VidAPI (dead)            |
| vaplayer.ru     | .ru | VidAPI **player**        |
| vidrock.ru      | .ru | VidRock                  |
| meowtv.ru       | .ru | MeowTV                   |
| hydrahd.ru      | .ru | HydraHD                  |
| vidstorm.ru     | .ru | VidStorm                 |

---

## 📐 Quick Reference: Common URL Patterns

```
# Pattern 1: /embed/movie/{id}  and  /embed/tv/{id}/{s}/{e}
# Used by: VidSrc family, VidCore, VidPlus, 2Embed.stream, AutoEmbed, VidAPI, 1Embed, etc.

# Pattern 2: /movie/{id}  and  /tv/{id}/{s}/{e}
# Used by: VidLink, VidFast, VidRock, VidNest, 111Movies, Videasy, etc.

# Pattern 3: ?id={tmdb}  and  ?id={tmdb}&s={n}&e={n}
# Used by: Embed-API, VidPop

# Pattern 4: ?video_id={id}  and  ?video_id={id}&s={n}&e={n}
# Used by: SuperEmbed/MultiEmbed

# Pattern 5: /embedtv/{id}&s={n}&e={n}
# Used by: 2Embed.cc, 2Embed.skin
```

```html
<!-- Universal iframe pattern -->
<iframe
  src="https://DOMAIN/PATH"
  width="100%"
  height="100%"
  frameborder="0"
  allowfullscreen
></iframe>
```

---

> **Sources:** Official sites, [vidsrc.domains](https://vidsrc.domains/),
> [vidapi.domains](https://vidapi.domains/), GitHub repositories
> ([TMDB-Embed-API](https://github.com/Inside4ndroid/TMDB-Embed-API),
> [CinePro](https://github.com/cinepro-org/backend),
> [EncDecEndpoints](https://github.com/smy778/EncDecEndpoints),
> [vidsrc-scraper](https://github.com/DivineChile/vidsrc-scraper)), community
> lists, direct endpoint verification. Status verified July 2026.

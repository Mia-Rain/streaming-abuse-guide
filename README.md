# Streaming Abuse Guide
A guide to abusing music streaming services like the trash they are.  

### Music Collection
When building a music collection, our best choice is typically Spotify. Spotify offers convenience along with algorithms that can produce good suggestions. This makes it the ideal tool for building a collection of music and playlists.  

See [Abusing Spotify](#abusing-spotify) for details on bypassing ads, limited features, and more when using a free account.

### Best Quality
While Spotify offers convenience, it only provides music at 320kbps with lossy OGG/MP3 compression at best. This is far worse than CD-quality music; a much better listening experience is easily achievable. High-quality lossless music is available from all other services except Soundcloud. This makes it extremely easy to rip songs from these platforms and play them locally.  
Below is a table of all the platforms, if they support lossless, their formats, and highest bits support should they have lossless.

| Platform  | Lossless  | Format  | Bits  |
|---  |---  |---  |---  |
| Deezer  | ✅   | Flac  | 24/16   |
| Tidal   | ✅   | Flac  | 24/16   |
| Amazon Music  | ✅   | Flac  | 24/16   |
| KKBOX   | ✅   | Flac  | 24/16   |
| Napster   | ✅   | Flac  | 16  |
| Apple Music   | ✅   | Alac in m4a   | 24/16   |
| Qobuz   | ✅   | Flac  | 24/16   |
| Spotify   | ❎   | ogg/mp3   | N/A   |
| Beatport  | ❎   | m4a   | N/A   |
| SoundCloud  | ❎   | Any   | N/A   |
| YouTube   | ❎   | Any   | N/A   |

### Pirating
Finally, we come to the fun part; Pirating! Obtaining music in DRM-free formats is easy if you know where to get it. My personal go-to is [doubledouble.top](https://doubledouble.top), but others such as [yams.tf](https://yams.tf) exist, but for the most up-to-date sources see [fmhy.net](https://fmhy.net). Additionally, tools for manually ripping tracks exist as well.  

Amazon Music, Deezer, and Qobuz are the best for gathering links as they don't require premium accounts to browse. Other platforms can be much harder to comb for music without a premium account.  

Below is info on abusing various platforms for the best experiences, junk for nerds about APIs, and sources for free account tokens.

---

### Abusing Spotify
For every platform that Spotify is present on, hacks and tools exist to bypass ads and spoof a premium account.
#### Desktop
On the desktop, there are tools just for bypassing ads. Still, those often don't work too well. [Spicetify](https://spicetify.app) can install extensions that bypass ads and provide premium features.
#### iOS
It's much easier to sideload using a jailbroken iPhone or one with [TrollStore](https://github.com/opa334/TrollStore). Methods for sideloading without these do exist, such as [sideloadly](https://sideloadly.io/) and [altstore](https://altstore.io/)/[sidestore](https://sidestore.io/). With that, it's possible to sideload the modified apps from [SpotCompiled](https://github.com/SpotCompiled).
#### Android
This really needs no guide. Endless "Spotify APK mod" downloads are all across the web.

---

### API junk/Free Premium Accounts

Below is various info on streaming APIs I've learned over time and some theories for sidestepping issues.

#### Spotify
Using the Web Playback SDK, Spotify Connect clients require a premium account. However, it should be possible to sidestep this by pretending to be a smart speaker and making spoofed requests with a bit of trickery to block ads.
#### Qobuz
Qobuz's API is no longer open source. However, it is still easy to abuse. Notably, API usage only requires a valid APP_ID and TOKEN. These never change. Allowing sources such as [firehawk32](https://rentry.org/firehawk52#tokens) to exist.
#### Deezer
Deezer uses a single cookie for Premium accounts. As such it's possible to modify it with the data from [firehawk32](https://rentry.org/firehawk52#deezer-arls)

All other platforms implement a proper OAuth API and thus aren't possible to bypass as far as I know.
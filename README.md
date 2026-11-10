# tv-playlist

Verified live TV playlist (M3U), re-checked weekly: every channel is probed
(real playlist + first segment fetch) before it stays on the list.
Channels marked (1080p) had their resolution measured from a real segment;
junk relays and channels measured below 1080p are removed. Unmarked channels
are alive-verified; their resolution could not be measured from the build host.

- Playlist: `list.m3u` — groups: 央视 / 卫视 / 体育 / 港澳台 / 地方其他
- EPG: declared in the playlist header (x-tvg-url), backup http://epg.51zmt.top:8000/e.xml

Subscribe URL:
https://raw.githubusercontent.com/lufeilaifu/tv-playlist/main/list.m3u

Test list (Shanghai China Mobile platform sources, playable only on Shanghai
Mobile networks - being verified on the captain's TV):
https://raw.githubusercontent.com/lufeilaifu/tv-playlist/main/test.m3u

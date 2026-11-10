# tv-playlist

Verified live TV playlist (M3U), re-checked weekly: every channel is probed
(real playlist + first segment fetch) before it stays on the list.

- Playlist: `list.m3u` — groups: 央视 / 卫视 / 体育 / 港澳台 / 地方其他 / 移动专线·待电视验证
- EPG: declared in the playlist header (x-tvg-url), backup http://epg.51zmt.top:8000/e.xml
- The last group （移动专线） holds China-Mobile IPv6 sources that can only be
  verified on a China Mobile network.

Subscribe URL:
https://raw.githubusercontent.com/lufeilaifu/tv-playlist/main/list.m3u

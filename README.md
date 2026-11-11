# tv-playlist

Live TV playlist (M3U), refreshed weekly from the Guovin iptv-api project
(Guangdong `gd` output). 715 entries (2026-11-11): 央视 / 卫视 / 体育 /
港澳台 / 上海、四川地方台. Source project verifies its own streams; entries
are published as-is, multiple backup URLs per channel.

Switched 2026-11-11 by the captain's instruction: the previous 392-channel
self-verified list (iptv-org / fanmingming / vbskycn sources, with (1080p)
labels and the epg.112114.xyz EPG header) was removed in full and replaced
by this upstream list.

Trimmed 2026-11-11 by the captain's instruction: all provincial local
groups except Shanghai and Sichuan removed (904 entries dropped from the
1,619-entry upstream list; Jiangxi has no local group upstream — only
江西卫视， kept inside the satellite group).

- Playlist: `list.m3u`
- EPG: declared in the playlist header (x-tvg-url, upstream Guovin epg.gz)

Subscribe URL:
https://raw.githubusercontent.com/lufeilaifu/tv-playlist/main/list.m3u

Test lists (being verified on the captain's TV):
- test.m3u: Shanghai Mobile platform sources (39.134 node) - played but too
  laggy in the 2026-11-10 TV test; kept for reference.
- test2.m3u: Migu (cmvideo) GSLB sources - TV test 2026-11-10: streams do not
  play (only the player's web-page fallback worked); dead, kept for reference.
- test3.m3u: GITV platform sources (223.110.241.139) via Jiangsu Mobile list -
  phone test 2026-11-10: playback fell back to the player's web-page source;
  the streams themselves are not validated. All three platform families
  (SH Mobile / Migu / GITV) failed as raw streams in third-party players.

# Firefox

- `about:config` is advanced preferences
- To get bookmarklets to work, `security.csp.enable` was set to `false`

## Quick Searches

To define your own quick search, add a bookmark with `%s` as the search term, then add a "Keyword".

## Downloading Video

Use "Video DownloadHelper", if it asks to use an external program (to download a `.m3u8`), just use this command instead:

	ffmpeg -protocol_whitelist file,http,https,tcp,tls,crypto -i "<.m3u8 video url>" -c copy video.mp4

## Share Menu

- Right-click a tab to access the share menu

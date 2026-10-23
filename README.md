# Enterprise AI News Studio

General enterprise-relevant AI news for Tim Hoyt, hosted on GitHub Pages.

- Site: https://miamirunning.github.io/claude-news-podcast/
- Feed: https://miamirunning.github.io/claude-news-podcast/feed.xml

In Apple Podcasts, open **Library > Follow a Show by URL** and paste the feed URL. The feed sets `itunes:block` to `yes`, so the show stays out of the Apple Podcasts directory and is available only by that URL.

`cover.jpg` is a simple placeholder (square JPEG). Replace that file when the illustrated cover is ready. Keep it square, RGB, and between 1400×1400 and 3000×3000 pixels. The feed already points at `cover.jpg`.

## Add a new episode

1. Copy the mp3 into `episodes/` (for example `episodes/ep02-example.mp3`). Keep the show notes beside it if you have them.
2. Record the exact file size in bytes (`wc -c < episodes/ep02-example.mp3`) and the duration.
3. Insert a new `<item>` as the first item in `feed.xml`:
   - `title` and a short `description`
   - `enclosure` with the full `https://miamirunning.github.io/claude-news-podcast/episodes/...` URL, `length` set to the byte size, and `type="audio/mpeg"`
   - a stable `guid` that will not change if you later replace the file
   - `pubDate` in RFC 822 (for example `Fri, 23 Oct 2026 17:00:00 GMT`)
   - `itunes:duration` (`HH:MM:SS` or whole seconds)
   - `itunes:episode` set to the episode number
   - `itunes:explicit` set to `false` unless the episode needs a warning
4. Add the episode to `index.html` if you want it on the site (an `<audio controls>` element is enough).
5. Commit and push to `main`. Pages serves the repository root, including `feed.xml`.

The enclosure `length` must match the mp3 on disk. Apple Podcasts rejects a feed when those numbers differ.

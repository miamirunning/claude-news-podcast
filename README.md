# Enterprise AI in Practice

Practical conversations about AI workflows, skills, plugins, and enterprise agents, hosted on GitHub Pages.

- Site: https://miamirunning.github.io/claude-news-podcast/
- Feed: https://miamirunning.github.io/claude-news-podcast/feed.xml

In Apple Podcasts, open **Library > Follow a Show by URL** and paste the feed URL. The feed sets `itunes:block` to `yes`, so the show stays out of the Apple Podcasts directory and is available only by that URL.

The current show artwork is `enterprise-ai-in-practice-cover-2026-10-26.png`, a 3000 × 3000 RGB PNG. Keep the feed and website on the same artwork URL. Use a fresh filename when replacing artwork so podcast players refresh their cache.

## Add a new episode

1. Copy the mp3 into `episodes/` (for example `episodes/descriptive-title-2026-10-26.mp3`). Keep the show notes beside it if you have them.
2. Record the exact file size in bytes (`wc -c < episodes/descriptive-title-2026-10-26.mp3`) and the duration.
3. Insert a new `<item>` as the first item in `feed.xml`:
   - `title` and a short `description`; use title and date without episode numbers
   - `enclosure` with the full `https://miamirunning.github.io/claude-news-podcast/episodes/...` URL, `length` set to the byte size, and `type="audio/mpeg"`
   - a stable `guid` that will not change if you later replace the file
   - `pubDate` in RFC 822 (for example `Fri, 23 Oct 2026 17:00:00 GMT`)
   - `itunes:duration` (`HH:MM:SS` or whole seconds)
   - `itunes:explicit` set to `false` unless the episode needs a warning
4. Add the episode to `index.html` if you want it on the site (an `<audio controls>` element is enough).
5. Commit and push to `main`. Pages serves the repository root, including `feed.xml`.

The enclosure `length` must match the mp3 on disk. Apple Podcasts rejects a feed when those numbers differ.

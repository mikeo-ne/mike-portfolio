# Mike 1ne — Portfolio

Static portfolio site for **Mike 1ne**, sound engineer / music producer / CEO of 7H Music Group (Kampala, Uganda).

Single-page, pure HTML/CSS/JS — no build step, no framework.

## Files

- `index.html` — the entire site
- `og-image.jpg` — social share preview (1200×630)
- `apple-touch-icon.png` — iOS home-screen icon
- `cover-llwymmd.jpg` / `.webp` — *Love Look What You Made Me Do* EP art
- `cover-ddna.jpg` / `.webp` — *Dance Di Night Away* single card photo
- `cover-different-patterns.jpg` / `.webp` — Tungi *Different Patterns* EP art
- `portrait-about.jpg` / `.webp` — About-section portrait
- `thumb-gas-station.jpg` / `.webp` — YouTube thumbnail for *Gas Station Freestyle*
- `.nojekyll` — tells GitHub Pages to serve files as-is (no Jekyll processing)

## Local preview

**Always preview through a local web server** — never by double-clicking
`index.html` (YouTube embeds require an HTTP Referer header, which browsers do
not send on `file://` URLs; opening the file directly will show a playback
configuration error on the YouTube card).

```bash
python3 -m http.server 8080 --bind 0.0.0.0
```

Then open http://localhost:8080 on any device on your network.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `mike1ne-portfolio`).
2. Upload **all** files from this folder to the repo (you can drag-and-drop the
   contents of `mike1ne-portfolio.zip` into the GitHub web UI, or use Git).
3. Go to the repo's **Settings → Pages**.
4. Under **Source**, pick the `main` branch and the `/ (root)` folder, then click
   **Save**.
5. Wait 30–60 seconds. Your site will be live at:
   - `https://<your-username>.github.io/mike1ne-portfolio/` if you used a repo named `mike1ne-portfolio`, or
   - `https://<your-username>.github.io/` if you deployed to a repo named `<your-username>.github.io`.
6. The `.nojekyll` file in this folder is required so GitHub serves the
   `apple-touch-icon.png` and `.webp` images without going through Jekyll.

Works out of the box on iPhone (Safari), Android (Chrome), Mac, and Windows.
All third-party embeds (Spotify, YouTube, Instagram) load lazily so the page is
fast on mobile networks.

## Contact

Bookings & inquiries: **mikeonerecords@gmail.com**
Instagram: [@mike.1ne_](https://www.instagram.com/mike.1ne_/)

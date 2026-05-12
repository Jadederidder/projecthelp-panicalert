# panicalert.projecthelp.co.za

Static install guide for the Bidvest Insurance Panic Alert app.
System fonts, no build step, ~1.2 MB total page weight.

## Files
- `index.html` — page (HTML + CSS + JS inline)
- `images/` — banner, hero side image, 3 real app screenshots
- `CNAME` — points GitHub Pages at `panicalert.projecthelp.co.za`

## Deploy
1. Create repo `Jadederidder/panicalert-site` (public).
2. Push these files to `main` (keep the `images/` folder structure intact).
3. Repo → Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)`.
4. DNS at Afrihost for `projecthelp.co.za`:
   - Type: `CNAME`
   - Host: `panicalert`
   - Target: `jadederidder.github.io.`
   - TTL: default
5. Wait ~10 minutes, then in Pages settings tick **Enforce HTTPS**.

`https://panicalert.projecthelp.co.za` will serve `index.html`.

## Editing
Everything visual is in one file. Open `index.html`, search for the section
you want (`HERO`, `INSIDE THE APP`, `INSTALL GUIDE`, etc.), edit, push to
`main`. Pages rebuilds in ~30 seconds.

## Image sources
- `banner.png` — Bidvest's existing PANIC ALERT email banner
- `hero-side.jpg` — Bidvest's existing menu background (masked figure + hand with app)
- `screen-test.png` / `screen-panic.png` / `screen-response.png` — real screenshots of the live Bidvest Panic Alert app

If Bidvest sends updated assets, replace files in `images/` keeping the same
filenames — the page picks them up automatically.

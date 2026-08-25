# Narita to Kansai

A nine-night Japan itinerary for two adults and two teenagers (17 and 14), Melbourne → Tokyo → Hakone → Kyoto → Osaka, 20–29 September 2026.

`index.html` is a single self-contained page. The only external request it makes is to Google Fonts; everything else — CSS, the theme toggle, the favicon — is inline, so it works from any static host with no build step.

## Publish it on GitHub Pages

```bash
git init
git add index.html README.md
git commit -m "Japan itinerary, September 2026"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

Then in the repository: **Settings → Pages → Build and deployment**, set *Source* to **Deploy from a branch**, choose **main** and the **/ (root)** folder, and save. The page goes live at:

```
https://YOUR-USERNAME.github.io/YOUR-REPO/
```

First deploy usually takes a minute or two. Every later `git push` republishes automatically.

Make the repository **public** if you want to share the link with people who don't have a GitHub account — Pages sites from private repositories are only reachable on paid plans.

## Other ways to host it

The file has no dependencies beyond the font request, so it also works as-is on Netlify Drop, Cloudflare Pages, Vercel, or an S3 bucket with static hosting turned on. You can also just open `index.html` in a browser, or email it — it renders offline, falling back to system fonts.

## Notes on the page itself

- **Themes.** Follows the reader's system light/dark setting by default. The toggle in the top-right overrides it and remembers the choice in `localStorage`.
- **Printing.** There's a dedicated print stylesheet — the toggle disappears, colours flatten to black on white, and days, tables and cards avoid breaking across pages. Print to PDF if you want a copy for the trip.
- **Editing.** Everything lives in one file. The palette is defined once as CSS custom properties in the `:root` block near the top, with dark-mode overrides directly below it, so recolouring means changing those values and nothing else.

## Accuracy

Prices were researched on 25 August 2026 at roughly A$1 = ¥114. Schedules, days of operation, rail pass prices, public holiday dates and attraction rules are verified against airline, JR, Odakyu and operator sources. Airfares are ranges drawn from aggregator route pages and airline "from" fares rather than live quotes — confirm at the time of booking. Hotel rates are recent midweek quotes and will price higher across Silver Week (19–23 September).

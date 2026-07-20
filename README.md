# Ayo Fashina — Media Kit Site

## What's in this folder
- `index.html` — the media kit / partnership proposal site (one page).
- `generator.html` — a tool to build a personalized link for each brand you pitch.
- `README.md` — this file.

## 1. Fill in your real content
Most of the site is already filled in with real content: the hero video, the Event Recap video, the Editorial Outfit Shots grid, and the Case Studies section all use real files from your `media/` folder.

The one thing still empty is the About portrait. Save your photo into `media/` as `about-portrait.png` (or `.jpg`), then replace this block:

```html
<div class="about-portrait ph-block"></div>
```

with:

```html
<div class="about-portrait" style="background:url('media/about-portrait.png') center/cover;"></div>
```

(Keep your image file in the same folder, or use a hosted image URL.) The same pattern works for any other photo on the site, swap the `background:url('media/your-file.png')` path any time you have newer or better photos to feature.

## 2. Put it online (so the link actually works for brands)
This needs a real public URL before you can send tailored links — right now it only works opened locally on your computer. Two free, no-code options:

**GitHub Pages** (best if you're comfortable with GitHub)
1. Create a new GitHub repo, upload `index.html` (and any photos).
2. Go to Settings → Pages → set source to the main branch.
3. Your site will be live at `https://yourusername.github.io/reponame/`.

**Netlify Drop** (fastest, zero setup)
1. Go to https://app.netlify.com/drop
2. Drag the whole `media-kit` folder onto the page.
3. Netlify gives you a live URL instantly (e.g. `https://random-name-123.netlify.app`).

Either way, once live, your media kit link is:
`https://your-live-url/index.html`

## 3. Send a tailored link to a brand
Open `generator.html` in your browser (double-click the file, no hosting needed for this tool). Paste your live site URL in the first field, fill in the brand's name, deliverables, and price, and click **Generate Tailored Link**. Copy the link it produces and send that to the brand instead of the plain homepage link — it will greet them by name/brand and show the specific plan you built for them.

You can also do this manually by adding to the end of your site URL:
```
?brand=Nike&contact=Jordan&deliverables=1%20Reel%20%2B%203%20Stories&price=%24950&note=Loved%20your%20Spring%20line
```

## 4. General vs. tailored
- Sending the plain link (no `?brand=...`) shows the general media kit — no public pricing, just a "custom proposals are scoped per partnership" statement — good for cold outreach or a media kit request.
- Sending a generated tailored link shows everything the plain link shows, PLUS a "Proposed Plan For [Brand]" section with the specific deliverables and price you set for that brand only — good once you're actually pitching a real partnership.

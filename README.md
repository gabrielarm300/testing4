# Gabriela Rodrigues de Morais — Portfolio (multi-page)

A software engineering portfolio with a hand-illustrated, cut-paper aesthetic — bold cutout lettering, taped Polaroid photos, and hand-drawn line-icon badges. Split across separate pages with real navigation.

## Files
- `index.html` — home page (hero with a Polaroid photo + "currently working on" whiteboard, plus a "have a look around" menu)
- `about.html` — about / bio
- `projects.html` — 8 real project write-ups with screenshots
- `interests.html` — placeholder ("under construction")
- `journey.html` — placeholder ("under construction")
- `contact.html` — placeholder ("under construction")
- `style.css` — all styling, shared by every page (colors/fonts are CSS variables at the top)
- `script.js` — gentle reveal animation on cards, shared by every page
- `assets/` — your photos and project screenshots

## 1. Personalize the content
- **index.html** — the whiteboard text ("Project I'm currently working on:"), hero subtitle, and the Polaroid photo/caption
- **about.html** — bio text and the three tag badges
- **projects.html** — edit each `.proj-polaroid` article directly: title, description paragraph(s), tag pills, and `img src`
- **interests.html / journey.html / contact.html** — currently just the "under construction" sign. When ready, replace the `<section id="...">...</section>` block with real content

## 2. Add more images
Drop new photos into the `assets/` folder and reference them with a relative path, e.g. `assets/project1.png`. Keep photos under ~1MB (compress/resize first) so pages load quickly.

## 3. Deploy to GitHub Pages
1. Create a new GitHub repository (e.g. `your-username.github.io` for a root domain, or any name like `portfolio`).
2. Push (or upload via the GitHub website) all the files **and the whole `assets/` folder** to the repo's root — or to a `/docs` folder if you prefer.
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Pick the `main` branch and the `/ (root)` folder (or `/docs` if that's where you put the files), then **Save**.
6. Wait a minute or two — GitHub will give you a live URL like `https://your-username.github.io/portfolio/`.

Quick command-line version:
```bash
git init
git add index.html about.html projects.html interests.html journey.html contact.html style.css script.js assets README.md
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin main
```
Then turn on Pages as described above.

## 4. Tweak the vibe
All colors and fonts live at the top of `style.css` under `:root` — change `--teal`, `--coral`, `--mustard`, etc. to shift the palette, or swap the Google Fonts links in each page's `<head>` for different fonts.

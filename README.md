# Nour Ben Said · Women Techmakers Ambassador Spotlight

A single-page spotlight for Nour Ben Said, built by Annet Sumi (Lava Rock Labs).

## Files

| File | What it is |
|---|---|
| `index.html` | The final page (denim and mustard design). Everything is inside this one file, including the photo. |
| `nour.jpg` | The cropped portrait, kept separately in case you want to swap or re-crop it. |
| `index-coastal.html` | Backup of the earlier coastal turquoise version. |

## Preview in VS Code

Open `index.html` and use the **Live Server** extension (right-click → *Open with Live Server*), or just double-click the file to open it in a browser.

## Publish on GitHub Pages

1. On github.com, create a **new public repository** named `nour-spotlight` (no README).
2. In this folder, in the VS Code terminal:
   ```
   git init
   git add index.html README.md
   git commit -m "Nour Ben Said WTM spotlight"
   git branch -M main
   git remote add origin https://github.com/<your-username>/nour-spotlight.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Branch: main, folder: /(root) → Save**.
4. After a minute or two the page is live at `https://<your-username>.github.io/nour-spotlight/`.

Wait to publish until Nour has approved the photo and quote.

## Still to do

- [ ] Nour approves using her photo (ideally she sends the original, uncropped photo; the current one is from a screenshot and the top of her hair is cut off)
- [ ] Nour approves the LinkedIn quote
- [ ] Add any details from her resume
- [ ] Add hobbies, music or a fun fact if she shares them
- [ ] Publish, then put the GitHub link in the email to Nour

## Swapping the photo

The photo is embedded in `index.html` as a long `data:image/jpeg;base64,...` string inside the `<div class="frame">`. To use a new photo, replace the whole `<img ...>` tag with:

```html
<img src="nour.jpg" alt="Portrait of Nour Ben Said, smiling">
```

and upload `nour.jpg` next to `index.html`. The frame is a 4:5 portrait shape, so a head-and-shoulders photo with a little space above the head works best.

## Design palette (from the fouta towel)

| Role | Hex |
|---|---|
| Background (soft white) | `#FAF9F6` |
| Text (deep denim) | `#2C3550` |
| Accent (denim blue) | `#4E5D86` |
| Stripe denim | `#667291` |
| Waffle denim | `#576385` |
| Light / highlight (mustard) | `#C9A04A` |
| Muted text | `#5C6480` |
| Lines | `#D3D8E3` |

Fonts: Schibsted Grotesk (text) and IBM Plex Mono (labels), from Google Fonts.

## Sources for the content

- Portfolio: https://nour-bensaid.github.io/my-portfolio/
- LinkedIn: https://www.linkedin.com/in/nour-bensaid/
- GitHub: https://github.com/nour-bensaid
- Interview with Nour, October 10, 2026

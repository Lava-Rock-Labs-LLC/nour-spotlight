# Nour Ben Said · Women Techmakers Ambassador Spotlight

A single-page spotlight for Nour Ben Said, built by Annet Sumi (Lava Rock Labs).

## Files

| File | What it is |
|---|---|
| `index.html` | The published page (denim and mustard design). Everything is inside this one file, including the photo. The "In her words" quote is left out for now. |
| `index-with-photo.html` | Local only. The full version with the "In her words" quote, ready to copy back in. |
| `nour.jpg` | Local only. The cropped portrait, kept separately in case you want to swap or re-crop it. |
| `index-coastal.html` | Local only. Backup of the earlier coastal turquoise version. |

The local-only files are listed in `.git/info/exclude`, so the repo itself stays two files.

## Preview in VS Code

Open `index.html` and use the **Live Server** extension (right-click → *Open with Live Server*), or just double-click the file to open it in a browser.

## Publish on GitHub Pages

This folder is connected to https://github.com/Lava-Rock-Labs-LLC/nour-spotlight. The page was pushed on October 12, 2026 with the photo Nour uses on her LinkedIn profile, but without the quote, since she hadn't replied yet.

1. On GitHub: **Settings → Pages → Branch: main, folder: /(root) → Save** (one time only).
2. After a minute or two the page is live at `https://lava-rock-labs-llc.github.io/nour-spotlight/`.
3. To publish later changes, in the VS Code terminal:
   ```
   git add index.html
   git commit -m "Describe the change"
   git push
   ```

## Still to do

- [x] Photo added (October 12, 2026, the same photo she uses on her LinkedIn profile)
- [ ] If Nour sends the original, uncropped photo, swap it in (the current one is from a screenshot and the top of her hair is cut off)
- [ ] Nour approves the LinkedIn quote
- [ ] Add any details from her resume
- [ ] Add hobbies, music or a fun fact if she shares them
- [x] Publish on GitHub Pages (October 12, 2026): https://lava-rock-labs-llc.github.io/nour-spotlight/
- [ ] Put the link in the email to Nour
- [ ] Post on LinkedIn, then add the link to the WTM tracker sheet

## Adding the quote back

Copy the `<section ... aria-label="In her words">` block from `index-with-photo.html` and paste it just above the "What's next" section in `index.html`. Then commit and push `index.html`.

## Swapping the photo

The photo is embedded in `index.html` as a long `data:image/jpeg;base64,...` string inside the `<div class="frame">`. To use a new photo, replace that line with:

```html
<div class="frame"><img src="nour.jpg" alt="Portrait of Nour Ben Said, smiling"></div>
```

and upload `nour.jpg` next to `index.html` (it's in `.git/info/exclude`, so remove it from there or use `git add -f nour.jpg`). The frame is a 4:5 portrait shape, so a head-and-shoulders photo with a little space above the head works best.

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

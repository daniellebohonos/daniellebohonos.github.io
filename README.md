# Danielle Bohonos — academic website

Clean, minimal academic site with dark-teal and dark-purple accents. Plain HTML/CSS,
no build step, so it hosts free on GitHub Pages (the same way chagaiweiss.com is hosted:
GitHub Pages + an optional custom domain).

## Pages
- `index.html` — home (photo, bio, research agenda, selected work)
- `publications.html` — peer-reviewed + non-peer-reviewed publications
- `working-papers.html` — working papers
- `government-experiences-study.html` — **the featured research-project page**; this is
  the participant-information page your business-card QR code should point to
- `teaching.html` — teaching experience
- `cv.pdf` — your CV (already copied in)
- `css/style.css` — all styling; accent colors are the variables at the top

## Still to do
1. **Add your headshot.** Save it as `images/photo.jpg`, then in `index.html` change
   `src="images/photo.svg"` to `src="images/photo.jpg"`.
2. **Add real links** where the entries say `<a href="#">` (Google Scholar profile URL,
   journal/DOI links).
3. Confirm the wording on `government-experiences-study.html` matches your REB-approved
   text exactly — a couple of fragments in the source doc were tidied for grammar.

## Preview locally
```bash
cd /Users/danielle/R-debug && python3 -m http.server 8000
```
Then open http://localhost:8000

## Publish on GitHub Pages
1. Create a repo named `yourusername.github.io` (e.g. `daniellebohonos.github.io`).
2. Push these files to the `main` branch.
3. Repo → Settings → Pages → Source: `main` / root.
4. Live at `https://yourusername.github.io`.
5. (Optional) Add a custom domain like `daniellebohonos.com` under Settings → Pages.
   The QR code on your business card can then point to
   `https://yourdomain/government-experiences-study.html`.

## Tuning the colors
Edit the top of `css/style.css`:
```css
--teal:   #0d5c63;
--purple: #4a2c6d;
```

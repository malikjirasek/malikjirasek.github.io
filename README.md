# Malik Jirasek — Academic Homepage

A clean, minimal academic personal website for GitHub Pages.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Landing page (bio, latest publication, news, contact) |
| `cv.html` | Online CV (full-page, linked to PDF download) |
| `publications.html` | Publications list |
| `projects.html` | Research projects |
| `interests.html` | Scientific & personal interests |
| `style.css` | All styles |
| `main.js` | Mobile nav + fade-in |
| `cv.pdf` | Downloadable PDF CV for applications |

## Deploying to GitHub Pages

1. Create a repository named **`your-username.github.io`** on GitHub (replace with your actual GitHub username).
2. Upload all files from this folder to the root of that repository.
3. In repository Settings → Pages → Source: select **main branch / root**.
4. Your site will be live at `https://your-username.github.io` within a minute.

> **Tip:** You can also use any other repo name (e.g. `homepage`) and the site will live at `https://your-username.github.io/homepage/`.

## Customising the Content

All placeholder text is marked with `[square brackets]` — just search for `[` in any editor to find everything you need to fill in.

### Priority checklist
- [ ] Replace `[your research focus]` in `index.html` (hero bio)
- [ ] Add your photo: replace the `<div class="avatar-placeholder">` with `<img src="photo.jpg" alt="Malik Jirasek">`
- [ ] Fill in your publications in both `index.html`, `publications.html`, and `cv.html`
- [ ] Update social profile links (GitHub, ORCID, Google Scholar, LinkedIn)
- [ ] Fill in education, research experience, skills in `cv.html`
- [ ] Regenerate `cv.pdf` after edits (see below)

## Updating the CV PDF

After you edit `cv_print.html` (the print-optimised version), regenerate the PDF:

```bash
pip install weasyprint
python3 -c "from weasyprint import HTML; HTML(filename='cv_print.html').write_pdf('cv.pdf')"
```

Or simply print `cv_print.html` from your browser (File → Print → Save as PDF) for a quick update.

## Adding Your Photo

Replace the placeholder div in `index.html`:
```html
<!-- Before -->
<div class="avatar-placeholder"><span>Photo</span></div>

<!-- After -->
<img src="photo.jpg" alt="Malik Jirasek" style="width:160px;height:200px;object-fit:cover;border-radius:2px;border:1px solid var(--rule);">
```

# alhernandezc.github.io

Personal site of **Adriana L. Hernández Castañeda**: economist & demographer.
Plain HTML/CSS, no build step, served by GitHub Pages.

## Deploy (one time, ~10 minutes)

1. **Rename this repo** to `alhernandezc.github.io`
   (repo → Settings → General → Repository name). This makes the site live at
   the root URL `https://alhernandezc.github.io` — which is what the CV,
   LinkedIn, and all internal links assume.
2. **Push these files** to the `main` branch (this whole folder is the repo root —
   `.nojekyll` included).
3. **Enable Pages**: Settings → Pages → Source: *Deploy from a branch* →
   Branch: `main`, folder `/ (root)` → Save.
4. Wait 1–2 minutes, then open **https://alhernandezc.github.io** and click
   every nav link, the two CV download buttons, and the Español toggle.

## Updating content

- Everything is hand-editable HTML. Shared styles live in `assets/style.css`.
- **When a research repo goes public**: in `projects.html` and `es/index.html`,
  each project card has a commented-out `links` block marked
  `<!-- TODO: uncomment when the repo is public -->` — uncomment it.
- **New CV version**: replace the PDFs in `assets/cv/` (keep the same filenames
  and everything keeps working).
- **ORCID / Google Scholar**: once Adriana creates the profiles, add the links in
  `index.html` (contact strip — there's a TODO comment) and to the `sameAs`
  array in the JSON-LD block at the top of `index.html`.

## Structure

```
index.html        Home (EN)
research.html     Publications, reports, memos
projects.html     Open-research project cards
cv.html           CV embed + downloads (EN/ES)
es/index.html     Spanish mirror (home + projects + contact)
assets/           style.css, favicon.svg, og.png, cv/*.pdf
404.html, robots.txt, sitemap.xml, .nojekyll
```

## Later (optional)

- Custom domain: buy one, add a `CNAME` file with the domain, set DNS per GitHub
  docs, keep HTTPS enforced.
- Analytics: GoatCounter or Plausible — one `<script>` line in each page.

# codesbyakhil.github.io — personal research site

A hand-built Jekyll site: research, experience, publications, blog (with LaTeX math
and Fortran syntax highlighting), and a dated news feed for research progress.
Designed to be hosted **free on GitHub Pages**.

---

## 1 · Deploy (one-time, ~10 minutes)

You need a GitHub account. Then:

1. **Create the repository.** On GitHub: *New repository* → name it exactly
   `codesbyakhil.github.io` (replace with your actual username) → Public → Create.
   This naming makes it a *user site*, served at `https://codesbyakhil.github.io`
   with no path prefix.

2. **Upload this folder's contents.** Two ways:
   - *Command line* (recommended):
     ```
     cd akhil-site
     git init
     git add .
     git commit -m "Initial site"
     git branch -M main
     git remote add origin https://github.com/codesbyakhil/codesbyakhil.github.io.git
     git push -u origin main
     ```
   - *Web upload*: on the empty repo page, "uploading an existing file" → drag
     everything in this folder (including the `_`-prefixed folders) → Commit.

3. **Enable Pages.** Repo → *Settings → Pages* → Source: **Deploy from a branch** →
   Branch: `main`, folder `/ (root)` → Save. GitHub builds the site with Jekyll
   automatically; it's live at `https://codesbyakhil.github.io` within a minute or two.

4. **Two small edits after deploy** (directly on GitHub or locally + push):
   - `_config.yml` → set `url: "https://codesbyakhil.github.io"` and fill in
     `links.github`.
   - Add your CV PDF at `assets/cv/akhil-s-pillai-cv.pdf` (delete the placeholder
     `.txt`).

> **Note on the build environment:** GitHub Pages builds with Jekyll **3.10** and a
> fixed plugin whitelist. This site uses only whitelisted plugins
> (`jekyll-seo-tag`, `jekyll-sitemap`, `jekyll-feed`) and 3.x-compatible templates,
> so it builds cleanly there. Don't add other plugins to `_config.yml` unless you
> switch to a GitHub Actions build.

---

## 2 · Everyday updates

### Add a news item (research progress — 30 seconds)
Edit `_data/news.yml`, copy a block to the **top**:
```yaml
- date: "Jul 2026"
  text: "Joined the Department of Aerospace Engineering at IIT Bombay as a PhD student."
```
Commit. Done. (A ready-made IITB template is already in the file, commented out.)

### Write a blog post
Create `_posts/YYYY-MM-DD-short-title.md`:
```markdown
---
title: "Post title"
subtitle: "Optional one-line standfirst."
tags: [dns, hpc]
---
Body in Markdown. Display math between $$ ... $$ on its own lines; inline math
as $$x$$ inside a sentence. Fenced code blocks with a language tag
(```fortran) get syntax highlighting.
```
MathJax loads automatically on every post. The filename date controls ordering.

### Add a research project
Copy one `<article class="project">…</article>` block in `research.md`, give it a
unique `id`, and edit. To show a figure (your vorticity renders will look great
here), drop an image into `assets/img/` and use the commented figure block —
captions follow the `Fig. n —` convention automatically.

### Update publications
Copy the commented block in `publications.md`. Link DOIs and PDFs as they exist.

### Photo
Drop `assets/img/akhil.jpg` and uncomment the `<img>` block in `index.html`.

---

## 3 · Local preview (optional)

Not required — you can edit on GitHub and let it build. For local preview:
```
gem install bundler && bundle install && bundle exec jekyll serve
```
then open http://localhost:4000. Requires Ruby ≥ 2.7.

---

## 4 · Structure

```
_config.yml          site settings, social links, build config
_data/news.yml       the news feed (edit this most often)
_layouts/            default / page / post templates
_includes/vortex.html  the Fig. 1 Kármán vortex street (hand-generated SVG)
_posts/              blog posts (Markdown)
index.html           homepage
research.md          projects
experience.md        roles, education, toolset
publications.md      thesis now; papers later
cv.md  blog/  404.html
assets/css/main.css  the entire design system (colors/type tokens at the top)
assets/cv/           put your CV PDF here
```

To change the accent colors or fonts site-wide, edit the `:root` variables at the
top of `assets/css/main.css` — everything derives from them.

---

## 5 · Later, if you want

- **Custom domain** (e.g. `akhilspillai.com`): buy from any registrar, add it in
  *Settings → Pages → Custom domain*, point DNS per GitHub's docs, keep
  "Enforce HTTPS" on. Hosting stays free; you pay only the registrar.
- **Google Scholar**: once your profile exists, paste the URL into
  `links.scholar` in `_config.yml` — it appears in the hero and footer automatically.
- **Thesis PDF**: if you host it, **redact personal details first** — the current
  PDF's resume page contains a home address and family phone number that should
  not go on the public web.

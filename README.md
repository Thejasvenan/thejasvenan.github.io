# Thejasvenan — Mechatronics Portfolio

This repository contains a GitHub Pages-ready static portfolio site for a Mechatronics engineer. It includes a responsive template (HTML/CSS) and an SVG illustration.

Files added:

- `index.html` — main site
- `css/style.css` — styles
- `assets/profile.svg` — hero illustration
- `index_alt.html` — alternate lighter variant for comparison
- `css/style_alt.css` — styles for the alternate variant

Preview locally

You can preview the site locally by opening `index.html` in your browser. For a better experience (serves files over HTTP) you can run a simple local server.

If you have Python 3 installed, run:

```powershell
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

Deploy to GitHub Pages

1. Commit and push these files to the `main` branch of this repository.
2. In GitHub, go to Settings → Pages and select "Deploy from a branch".
3. Choose the `main` branch and the `/ (root)` folder, save.
4. After a minute, your site will be available at `https://thejasvenan.github.io/` (or the URL GitHub shows).

Compare the two styles

- `index.html` + `css/style.css` — darker, polished engineering theme with cards and a stronger design presence. Good for a professional/mechatronics portfolio emphasizing projects and visuals.
- `index_alt.html` + `css/style_alt.css` — lighter, more personal resume-like layout with straightforward lists and text. Good for a fast-read, mobile-friendly personal page.

Recommendation: For a Mechatronics + AI portfolio, the darker, card-style `index.html` offers better visual hierarchy for projects and technical content. Use `index_alt.html` if you prefer a minimal, resume-first presentation.

Customization

- Replace the placeholder email and links in `index.html`.
- Add project images to `assets/` and update project cards.
- Add project images to `assets/projects/` and create per-project Markdown files under `projects/`.

Projects structure (Jekyll-friendly)

- `projects.md` — overview page listing projects
- `projects/<slug>.md` — per-project page with front matter and content (example pages already added)
- `assets/projects/<project>-thumb.svg|png|jpg` — thumbnail images

To add a new project:

1. Create `projects/<your-slug>.md` with front matter:

```yaml
---
title: Your Project Title
layout: default
permalink: /projects/your-slug/
---
```

2. Add your content, insert images stored under `assets/projects/`, and link a GitHub repo.

Media tips

- Add images (PNG/JPG) and short demo videos (MP4) to `assets/projects/` and reference them in the project Markdown. Example usage is included in the sample project pages.
- Add your CV (PDF) to `assets/` and name it `CV-Thejasvenan.pdf` (or update the `href` in `index.html` to match).

To update the CV link:

1. Place your PDF at `assets/CV-Thejasvenan.pdf`.
2. Or open `index.html` and change the `href` values that point to `assets/CV-Thejasvenan.pdf` to your PDF filename.

License

This template is free to use and customize.

# thejasvenan.github.io

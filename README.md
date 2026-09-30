# Academic Website Starter Kit

A Quarto website modeled on the clean academic style of
waitkus.github.io, adapted for a **teaching-focused** job market
(nav order leads with Teaching).

## What's in here

```
mysite/
├── _quarto.yml      ← site config: your name, nav, theme, footer icons
├── index.qmd        ← landing page (photo + short bio)
├── about.qmd        ← background, education
├── teaching.qmd     ← philosophy, courses, syllabi, evidence  ★ the key page
├── research.qmd     ← publications & presentations
├── cv.qmd           ← embedded + downloadable CV
├── styles.css       ← light styling tweaks (accent color, spacing)
├── assets/          ← put headshot.jpg here
└── files/           ← put cv.pdf, syllabi PDFs, teaching philosophy PDF here
```

## Step 1 — Install the tools (one time)

1. Install Quarto: https://quarto.org/docs/get-started/
2. (Optional but nice) Install VS Code or RStudio to edit files.
3. Install Git and create a free account at https://github.com

## Step 2 — Personalize

Search the files for these placeholders and replace them:

- `Your Name` — everywhere
- `you@university.edu` — your email
- `YOUR_ID` — your Google Scholar profile ID (the string after
  `user=` in your Scholar profile URL)
- `0000-0000-0000-0000` — your ORCID
- ~~GitHub username~~ — already filled in for you (top1016)

Then add your real files:

- `assets/headshot.jpg` — a professional photo (square works best)
- `files/cv.pdf`
- `files/teaching-philosophy.pdf`
- `files/syllabus-sample.pdf` (and any others; update links in
  `teaching.qmd` to match your filenames)

Every `.qmd` file contains `<!-- comments -->` with writing guidance.
Delete the comments as you fill in real content.

## Step 3 — Preview locally

From this folder, run:

```
quarto preview
```

A browser window opens showing the site; it live-reloads as you edit.

## Step 4 — Publish to GitHub Pages (free)

1. On GitHub, create a new **public** repository named exactly:
   `top1016.github.io`
2. In this folder, run:

```
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/top1016/top1016.github.io.git
git push -u origin main
quarto publish gh-pages
```

3. Confirm the prompts. In a few minutes your site is live at
   `https://top1016.github.io`

## Updating the site later

Edit files → `quarto preview` to check → then:

```
git add . && git commit -m "Update"
git push
quarto publish gh-pages
```

## Nice-to-haves later

- **Custom domain** (~$12/yr): buy `yourname.com`, then follow
  https://quarto.org/docs/publishing/github-pages.html#custom-domain
- **Themes**: swap `flatly`/`darkly` in `_quarto.yml` for any pair
  from https://quarto.org/docs/output-formats/html-themes.html
- **Analytics-free by design** — committees appreciate fast, simple.

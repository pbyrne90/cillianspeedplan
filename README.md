# Cillian's Speed Plan

A simple, self-contained website for Cillian's twice-a-week rugby / field-sport speed plan.
Built as a single static `index.html` file — no build step, no dependencies.

**Live site:** https://pbyrne90.github.io/cillianspeedplan/

## Files

- `index.html` — the whole website (HTML + CSS in one file).
- `cillians_speed_plan.md` — the original source plan the site is built from.
- `.nojekyll` — tells GitHub Pages to serve the files as-is.

## How to publish it to GitHub Pages

You only need to do this once. The repo must be named **`cillianspeedplan`** and owned by **`pbyrne90`** for the URL above to work.

### Option A — via the GitHub website (no command line)

1. Go to https://github.com/new and create a new **public** repository named `cillianspeedplan`.
2. On the new empty repo page, click **uploading an existing file**.
3. Drag in `index.html`, `README.md`, `cillians_speed_plan.md`, and `.nojekyll`, then **Commit**.
4. Go to **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **Deploy from a branch**.
6. Set the branch to **`main`** and the folder to **`/ (root)`**, then **Save**.
7. Wait 1–2 minutes. The site goes live at **https://pbyrne90.github.io/cillianspeedplan/**

### Option B — via git on the command line

From inside this folder:

```bash
git init
git add .
git commit -m "Cillian's Speed Plan website"
git branch -M main
git remote add origin https://github.com/pbyrne90/cillianspeedplan.git
git push -u origin main
```

Then follow steps 4–7 from Option A to turn on GitHub Pages.

## Editing the content later

All the text lives in `index.html` inside the `<section>` blocks. Edit the text, save,
re-upload (or `git commit` + `git push`), and the live site updates within a minute or two.

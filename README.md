# mindfulmovement.github.io

A minimal personal site: a landing page and a blog. GitHub Pages builds it automatically with Jekyll, so you only edit Markdown files.

## What's where

| File / folder | What it is |
|---|---|
| `index.md` | Landing page (photo + text) |
| `assets/images/portrait.svg` | Placeholder photo. Replace it with your own (e.g. `portrait.jpg`) and update the filename in `index.md` |
| `_posts/` | Blog posts. One Markdown file per post |
| `blog.html` | The blog list page (you won't need to touch it) |
| `_config.yml` | Site title, author, description |
| `assets/style.css` | All styling |
| `_templates/` | Obsidian template for new posts (not published) |

## Writing a post

1. Create a file in `_posts/` named `YYYY-MM-DD-short-title.md`, e.g. `2026-11-02-why-i-train-slowly.md`. The date prefix is required; the rest becomes the URL (`/blog/why-i-train-slowly/`). Use lowercase and hyphens, no spaces.
2. Start it with:

   ```
   ---
   title: Why I train slowly
   ---
   ```

3. Write below in normal Markdown. Save, commit, push. The site updates within about a minute.

## Using Obsidian

Open this folder as a vault (Obsidian → Open folder as vault). It comes preconfigured so that:

- New notes go into `_posts/`
- Pasted images go into `assets/images/` and use normal Markdown links (not `[[wikilinks]]`), which work on the site
- The **Templates** core plugin uses `_templates/`. Enable it under Settings → Core plugins → Templates, then use "Insert template" → "New post" in an empty note

Things to avoid: `[[wikilinks]]` to other notes and Obsidian-only syntax (callouts, embeds) won't render on the site.

The `.obsidian/` settings folder is never published.

## First-time setup

1. In the `mindfulmovement` organization on GitHub, create a **public** repository named exactly `mindfulmovement.github.io`.
2. Upload these files (see options below).
3. Repo → Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`, Save.
4. Visit https://mindfulmovement.github.io/ after a minute or two.

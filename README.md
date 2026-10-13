# fredrin-ayush-portfolio

A small, hand-written portfolio site for **Ayush Mania** (forward deployed
engineer and platform architect), built as a Fredrin project for an FDE
application.

## Live pages

Both were checked and return HTTP 200 (GitHub Pages, built from `main`):

| Page | URL |
|---|---|
| About Me - who Ayush is, work history, projects | https://ayush-mania.github.io/fredrin-ayush-portfolio/ |
| How this was made - the ticket chain and honest notes | https://ayush-mania.github.io/fredrin-ayush-portfolio/work.html |

Source repository: https://github.com/ayush-mania/fredrin-ayush-portfolio

The owner's main portfolio (a separate project, not part of this repo) is at
https://ayush-mania.vercel.app.

## What is in the repo

| Path | Purpose |
|---|---|
| `index.html` | About Me page |
| `work.html` | Plain-language explanation of how the site was planned and built |
| `assets/style.css` | Shared stylesheet |
| `data/owner.json` | Identity, links, intro, experience, education |
| `data/projects.json` | The six portfolio projects |
| `.nojekyll` | Tells GitHub Pages to publish the files as-is (no Jekyll) |

Plain HTML and CSS. No build step, no dependencies, no JavaScript framework.
The pages are written by hand; `data/` is the source of facts they draw on.

## Content and sources

Owner and project facts come from the source portfolio repository
(https://github.com/ayush-mania/portfolio) and nothing else. Several TestDino
figures there are marked unverified or disputed, so `data/projects.json`
carries that caveat instead of restating them as fact.

## Run locally

No install needed. Open `index.html` in a browser, or serve the folder:

```sh
git clone https://github.com/ayush-mania/fredrin-ayush-portfolio.git
cd fredrin-ayush-portfolio
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deployment

GitHub Pages deploys straight from a branch, with no GitHub Actions workflow.

- Source: branch **`main`**, folder `/ (root)` (confirmed via the repository's
  Pages settings).
- Flow: merge a PR into `main` and Pages republishes. Other branches never
  deploy.
- If Pages is ever reset: Settings -> Pages -> Source: **Deploy from a
  branch** -> `main`, `/ (root)`.

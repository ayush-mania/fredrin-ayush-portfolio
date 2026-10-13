# fredrin-ayush-portfolio

Ayush Mania's personal portfolio.

## Status

A hand-written static site: `index.html` (About Me), `work.html` (how it was
made, in plain language), `assets/style.css`. No build step, no dependencies.

## Deployment

Deployed by GitHub Pages straight from a branch, with no GitHub Actions
workflow, so it uses no Actions minutes.

- Deploy branch: **`main`**, folder `/ (root)`. It is the only source.
- Flow: merge a PR into `main` -> Pages publishes the files as-is
  (`.nojekyll` skips the Jekyll build). Other branches never deploy.
- One-time setup: Settings -> Pages -> Source: **Deploy from a branch** ->
  Branch `main`, `/ (root)`. If it was set to "GitHub Actions", switch it.

Live links (404 until the setup above is done):

- What was built: https://ayush-mania.github.io/fredrin-ayush-portfolio/
- How it was done: https://ayush-mania.github.io/fredrin-ayush-portfolio/work.html

## Content

Owner and project facts live in `data/`, taken from the source portfolio
repository (https://github.com/ayush-mania/portfolio) and nothing else:

- `data/owner.json` - identity, links, intro, experience, education
- `data/projects.json` - the six portfolio projects

Several TestDino figures in the source are marked unverified or disputed there;
`data/projects.json` carries that caveat rather than restating them as fact.

## Getting the code

```sh
git clone https://github.com/ayush-mania/fredrin-ayush-portfolio.git
cd fredrin-ayush-portfolio
```

## Install and run locally

No install needed. Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

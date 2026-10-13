# fredrin-ayush-portfolio

Ayush Mania's personal portfolio.

## Status

A hand-written static site: `index.html` (About Me), `work.html` (how it was
made, in plain language), `assets/style.css`. No build step, no dependencies.

Live links. These return 404 until GitHub Pages is switched on once:
Settings -> Pages -> Source: **GitHub Actions** (`.github/workflows/pages.yml`
then publishes every push to `main`). Alternatively choose Deploy from branch
`main`, folder `/ (root)` and ignore the workflow:

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

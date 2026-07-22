# Site setup

## License

The site's code and design (layouts, includes, CSS) are MIT licensed --
see `LICENSE`. Written content (page text, project write-ups, posts) is
all rights reserved and not covered by that license.


A custom Jekyll site (no third-party theme -- layouts and CSS are all
in this repo) meant to be pushed to a repo named exactly
`<your-username>.github.io` and served via GitHub Pages.

## To publish

1. Create a GitHub repo named `signal-within-noise.github.io`.
2. Push all files in this folder to the `main` branch.
3. In the repo's Settings -> Pages, set source to "Deploy from a branch",
   branch `main`, folder `/ (root)`.
4. Your site will be live at `https://signal-within-noise.github.io`
   within a few minutes.

## Structure

- `index.md` -- About Me (home page). Uses the `home` layout; edit the
  front matter (eyebrow, headline, credentials, links) and the body
  text for your bio.
- `_layouts/` + `_includes/` -- the custom design (nav, waveform, panels,
  typography). `assets/css/style.css` is the one stylesheet.
- `writing.md` + `_posts/` -- the blog section. Add a new file to
  `_posts/` (format `YYYY-MM-DD-title.md`, front matter `layout: post`)
  each time you write something new -- it appears on `/writing/`
  automatically.
- `projects/` -- one page per project (`layout: page`), plus
  `projects/index.md` which lists them as panels. To add a project:
  1. Create `projects/your-project.md` (copy `svd-mortality.md` as a template)
  2. Add an entry to `_data/projects.yml` so it shows up on the projects list
- `assets/images/` -- chart PNGs referenced by project pages.

## Adding your chart images

Copy `observed_vs_predicted.png`, `agg_mort.png`, and `svd_reconst_mort.png`
into `assets/images/` before pushing -- they're referenced by
`projects/svd-mortality.md` and the projects list thumbnail, but not
included in this scaffold.

## Local preview (optional)

```
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`. Not required -- GitHub rebuilds the
site automatically on every push either way.

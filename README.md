# kirpitch-site

Static site for https://kirpitch.dev, the home of [Kirpitch](https://github.com/cocan-dev/kirpitch).
Plain HTML and CSS plus two small inline scripts (the light/dark theme switch and a
decorative hero background). No build tools, no cookies, no analytics, no
third-party requests. The only thing stored is the theme choice in the visitor's
own browser. Hosted on GitHub Pages.

- Preview locally: `python -m http.server 8080` in this folder.
- `.github/workflows/deploy.yml` deploys the site on every push to `main`.
- The workflow copies a fixed list of files. If you add or remove a file the site
  needs, change the `cp` line in `deploy.yml` in the same commit.
- Pages must use the "GitHub Actions" source in the repo settings.
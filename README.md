# kagent @ KubeCon + CloudNativeCon Japan

Landing page for the kagent hands-on labs, presented at KubeCon + CloudNativeCon Japan.
Built with [Hugo](https://gohugo.io/) (extended) and deployed to GitHub Pages.

**Live:** https://solo-io.github.io/kubecon-2026-japan-labs/

## Local development

```bash
hugo server -D
# http://localhost:1313/
```

## Editing the labs

All four lab tiles are data-driven — edit `data/labs.yaml` to change titles,
descriptions, tags, or `url`s. No template changes required.

## Deploy

Pushing to `main` triggers the `.github/workflows/hugo.yml` workflow, which builds
the site and publishes it to GitHub Pages. Enable Pages once under
**Settings → Pages → Build and deployment → Source: GitHub Actions**.

## Structure

```
hugo.toml                 # site config + event params
data/labs.yaml            # the 4 lab tiles (edit here)
layouts/index.html        # landing page
layouts/_default/baseof.html
layouts/partials/icon.html
assets/css/main.css       # all styling
```

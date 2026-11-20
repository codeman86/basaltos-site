# BasaltOS site

Public website for BasaltOS, a hardened Linux OS based on Debian stable.

The site is plain HTML and CSS. There is no build step, no tracker, and no CDN. Open `index.html` in a browser, or from this directory:

```bash
python3 -m http.server 8080
```

Pages: Home, Features, Editions, Download, Roadmap, About. Links are relative so the same files work at `https://codeman86.github.io/basaltos-site/` and on any static host that serves the repository root.

Strata screenshots are referenced from `assets/` under these names:

- `basaltos-boot-splash.png`
- `basaltos-login-screen.png`
- `basaltos-desktop-m2.png`
- `basaltos-logo-start-button.png`
- `basaltos-wallpapers-contact-sheet.png`

## GitHub Pages

Deploys from `main` with GitHub Actions (`.github/workflows/pages.yml`).

In the repository settings, set Pages → Build and deployment → Source to **GitHub Actions**. The workflow does not run as the Pages source until that setting is on.

## Vercel

The repository root is a static site. Vercel can deploy it with zero configuration: no `vercel.json`, no install, no build command.

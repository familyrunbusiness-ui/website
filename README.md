# William Pollard

Static portfolio website for artist William Pollard.

**Live site:** [www.williampollard.com](https://www.williampollard.com/)

## About

This repository contains the source files for the William Pollard portfolio website. It is a lightweight static site built with HTML and CSS and published through GitHub Pages.

## Project structure

- `index.html` — home page
- `styles.css` — shared site styling
- `assets/` — images and other media
- `bio/` — biography/about page
- `work-visual/` — visual work and portfolio page
- `CNAME` — GitHub Pages custom-domain configuration
- `.nojekyll` — serves the files directly without Jekyll processing

## Local preview

No build step or package installation is required. From the repository root, run:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a browser.

## Deployment

GitHub Pages publishes the `main` branch from the repository root. Changes committed to `main` are deployed automatically.

The production site uses `www.williampollard.com` as its custom domain, with HTTPS enforced. The apex domain, `williampollard.com`, redirects to the `www` address.

## DNS records

To keep the custom domain connected to GitHub Pages, the DNS provider must retain these records:

| Type | Host | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `familyrunbusiness-ui.github.io` |

When moving the domain to another registrar or DNS provider, copy these records before changing nameservers to avoid downtime.

## Updating the site

1. Edit the relevant HTML, CSS, or asset files.
2. Preview the changes locally.
3. Commit the changes to `main`.
4. Confirm the deployment in the repository's **Actions** or **Deployments** section.


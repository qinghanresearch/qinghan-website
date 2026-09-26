# Qing Han personal website

A Quarto website with custom CSS and 19 academic and professional profile pages.

## Local preview

```sh
quarto preview --host 127.0.0.1 --port 4200 --no-browser
```

On this Mac Quarto is also available at `/Applications/quarto/bin/quarto`.

## Publish with GitHub Pages

1. Publish this repository (only `qinghan-website`, never its parent materials folder) using GitHub Desktop. Use a public repository for GitHub Pages on GitHub Free.
2. In the GitHub repository, select **Settings → Pages → Source → GitHub Actions**.
3. Open **Actions → Publish website → Run workflow**. Later pushes to `main` rebuild and deploy automatically.

The workflow installs Quarto 1.10.18, renders the site, and deploys only `_site`. It obtains the actual website URL from GitHub Pages for canonical links and the sitemap. No access token needs to be stored in this repository.

The public repository is https://github.com/qinghanresearch/qinghan-website and the live website is https://qinghanresearch.github.io/qinghan-website/. GitHub Pages deploys automatically after a push to main. No custom domain is configured. For a custom domain, configure it in GitHub Pages and with the DNS provider after the default address works.

## Editing and evidence

Main navigation pages are at the root; detail pages are in `research/`, `projects/`, and `writing/`. Edit `styles.css` for presentation and `_quarto.yml` for navigation. See `AGENTS.md` for the user's editorial rules.

Only the portrait, favicon, and book photograph are included as public assets. Unused photographs and conceptual artwork remain locally excluded from Git and explicit render resources. CV printing uses the browser's print dialog.

## Publication boundary

Do not import the parent folder or publish private applications, fieldnotes, business plans, contracts, credentials, or complete evidence dossiers. Search indexing is enabled for launch. The publisher of *The Ancient Hongshan Kingdom* is Jilin University Press (吉林大学出版社), confirmed by Qing Han.

Deployment references: [Quarto GitHub Pages](https://quarto.org/docs/publishing/github-pages.html), [GitHub Pages workflows](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).

## Routine content updates

Keep source materials outside this repository. Prepare public summaries in the relevant `.qmd` pages, preview locally, check related homepage/Research/Writing/CV entries, then commit and push the reviewed changes. Confirm the Publish website workflow succeeds before treating an update as live.

`research/hongshan.qmd` now presents **Translation as Governance**; its established URL is retained. Research proposals and pilot analyses must be identified as work in progress. Private source notes and unverified claims must not be copied into public pages.

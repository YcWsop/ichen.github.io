# Research homepage

A single responsive static page. No build or external assets required.

## Files

- index.html: research overview and project stage labels.
- .nojekyll: disable Jekyll processing.

## Project status

These are conservative descriptions of the current work stage. Availability of
public files is a separate question from completion of the underlying work.

| Project | Stage shown on the homepage | Public materials |
| --- | --- | --- |
| LangevinFlow | Presentation stage; writing in preparation | No manuscript or code linked yet |
| Monte Carlo random matrix | Simulation / presentation stage | Code and presentation release pending |
| Spin glass | Notes / draft stage | Final public version pending |
| Statistical mechanics of transfer learning | Study stage; follow-up planned | Research scope not finalized; no completed follow-up results claimed |

## Deployment check: 11 October 2026

- The `main` branch contains `index.html`, `.nojekyll`, and this README.
- The public repository metadata reports `has_pages: false`.
- The expected project-site address returns HTTP 404.
- The GitHub connection supports repository file writes, but exposes no Pages
  settings API. The Pages settings page in the available browser requires login.

The files are ready for static hosting. Follow the steps below to enable
publication; a committed homepage alone does not turn on GitHub Pages.

## Publication

1. Open https://github.com/YcWsop/ichen.github.io/settings/pages
2. Select Deploy from a branch, main, / (root), then Save.
3. Wait for the Pages build and verify https://ycwsop.github.io/ichen.github.io/
   Confirm that the page shows all four project headings; check the Actions tab
   if the deployment fails.

This repository is a project site: its name is not ycwsop.github.io.
Do not assume https://ichen.github.io/ belongs to this account.

Official instructions:

- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Content maintenance

Stage labels are a conservative snapshot, not publication or completed research claims.
Review them as work progresses. Add actual public materials before adding download links.
Notes section is reserved for future posts; no empty links or invented CV/contact details.

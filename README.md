<p align="center">
  <img alt="FuseScope" src=".github/brand/fusescope-logo-universal.svg" width="440">
</p>

<h1 align="center">FuseScope site</h1>

<p align="center">
  <b>The FuseScope landing page.</b>
</p>

<p align="center">
  <a href="https://fusescope.fuseone.io">fusescope.fuseone.io</a> ·
  <a href="LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-0f5fb8"></a>
  <a href="https://github.com/fuseone-io/fusescope-site/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/fuseone-io/fusescope-site?color=950fb8"></a>
</p>

The landing page at [fusescope.fuseone.io](https://fusescope.fuseone.io): static files in `public/`, no build step.
Deployed as a Cloudflare Worker with static assets (`wrangler.jsonc`) by `.github/workflows/deploy.yml` on every
push to `main` (secrets `CLOUDFLARE_API_TOKEN`, `CLOUDFLARE_ACCOUNT_ID`);
`public/_headers` sets the security headers and asset caching.

The page was designed on the FuseScope design canvas and exported to plain HTML. Logos in `assets/` come from
`fuseone-io/fusescope` `docs/brand/`; reuse them, never redraw.

Preview locally:

```sh
python3 -m http.server 8000 -d public
```

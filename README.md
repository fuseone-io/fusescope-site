# FuseScope site

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

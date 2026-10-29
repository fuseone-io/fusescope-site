# FuseScope site

The landing page at [fusescope.fuseone.io](https://fusescope.fuseone.io): one static `index.html`, no build step.
Hosted on Cloudflare Pages from `main`; `_headers` sets the security headers and asset caching.

The page was designed on the FuseScope design canvas and exported to plain HTML. Logos in `assets/` come from
`fuseone-io/fusescope` `docs/brand/`; reuse them, never redraw.

Preview locally:

```sh
python3 -m http.server 8000
```

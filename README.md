# cdn (public)

Production assets for Superpresence Webflow projects, served via jsDelivr.
Source lives in the private `Superpresence-Co/Clients` repo.

**Public repo — NEVER commit secrets.**

## URL format
```
https://cdn.jsdelivr.net/gh/Superpresence-Co/cdn@<tag>/<client>/script.js
```
Tags: `<client>-vX.Y.Z` (e.g. `onelisted-v2-v1.0.0`). Always pin a tag in Webflow; never use `@main` in production (cached up to 12h, and changes go live unreviewed).

## Release
```bash
git add <client>/ && git commit -m "<client>: describe change"
git tag <client>-v1.0.1 && git push && git push --tags
```

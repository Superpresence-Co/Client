# cdn (public)

Production code for Superpresence client Webflow projects, served via jsDelivr.
One folder per client. Only code delivered to the client lives here; prototyping happens in CodeSandbox.

**Public repo: NEVER commit API keys/tokens, and no internal notes or links (keep those in internal docs).**

| Folder | Project |
|---|---|
| `superpresence-v2.5/` | Superpresence V2.5 |
| `onelisted-v2/` | Onelisted V2 |

Folder names: lowercase, kebab-case. Each client folder has `script.js`, `style.css`, and a README with the Webflow embed code + changelog.

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

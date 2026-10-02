# Client

Final code (script & style) for Superpresence clients' Webflow websites.
One folder = one client. Each folder contains only `script.js` and `style.css`.

Testing happens in CodeSandbox. Code is added here only after it has been delivered to the client.

> ⚠️ This repo is **public**. Never store passwords, API keys, or internal notes here.

## Example: Webflow embed code
Replace `client-name` with the client's folder name and `v1.0.0` with the version you want.
Paste in Webflow → Site settings → Custom code.

Paste in **Head**:
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Superpresence-Co/Client@client-name-v1.0.0/client-name/style.css">
```
Paste before **</body>**:
```html
<script src="https://cdn.jsdelivr.net/gh/Superpresence-Co/Client@client-name-v1.0.0/client-name/script.js" defer></script>
```

## Updating a client's code
1. Update `script.js` / `style.css` in the client's folder.
2. Commit & push.
3. Create a new version, e.g. `git tag client-name-v1.0.1 && git push --tags`
4. In Webflow, change `v1.0.0` in the embed links to the new version.

Always use a version number in the links. Don't use `@main`: changes can show up late (cached for up to 12 hours) and go live without review.

## Adding a new client
Create a new folder using lowercase letters and `-` (e.g. `client-name-v1`), add `script.js` and `style.css`.

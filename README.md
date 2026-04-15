# PasteReady Legal

Legal pages for the [PasteReady](https://github.com/BaklazhenkoNikita/IDonce) app, hosted via GitHub Pages.

## Live URLs

| Page | URL |
|------|-----|
| Landing | https://baklazhenkonikita.github.io/pasteready-legal/ |
| Privacy Policy | https://baklazhenkonikita.github.io/pasteready-legal/privacy |
| Terms of Service | https://baklazhenkonikita.github.io/pasteready-legal/terms |
| Data Deletion | https://baklazhenkonikita.github.io/pasteready-legal/data-deletion |

## How to Update

Edit the markdown files and push:

```bash
git add -A && git commit -m "Update legal pages" && git push
```

GitHub Pages rebuilds automatically on push. Changes go live within a few minutes.

## Structure

```
_config.yml       — Jekyll theme config (minima)
index.md          — Landing page linking to all documents
privacy.md        — Privacy Policy
terms.md          — Terms of Service
data-deletion.md  — Data Deletion Instructions
```

# PR Review Request — Simple HTML Version

No build step, no dependencies. Just open `index.html` in a browser.

## How to run

### Option 1 — Open directly in browser
```
open /Users/exaacy/copilot_play/teams-pr-form-simple/index.html
```

### Option 2 — Serve locally (avoids CORS issues)
```bash
npx serve .
```
Then open http://localhost:3000

## Comparison vs React version

| | React version (`teams-pr-form/`) | Simple version (`teams-pr-form-simple/`) |
|---|---|---|
| **Dependencies** | 136 npm packages | Zero |
| **Build step** | `npm run build` required | None |
| **Run locally** | `npm run dev` | Just open `index.html` |
| **Deploy** | Upload `dist/` folder | Upload single `index.html` |
| **Customise** | Edit JSX + rebuild | Edit HTML directly |
| **Teams SDK** | ✅ Included | ❌ Not included |

## Deploy for your team

Just upload `index.html` to any static host — even a SharePoint page or GitHub Gist works.

For Netlify:
```bash
npx netlify-cli deploy --dir=. --prod
```

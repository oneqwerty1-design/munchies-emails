# Connect to Vercel — 2 steps left

Remote is already configured:
`origin → https://github.com/oneqwerty1-design/munchies-emails.git`

## 1. Push (needs your GitHub credentials)

From inside this folder:

```bash
git push -u origin main
```

If it asks for a password, GitHub wants a Personal Access Token, not your
account password — github.com/settings/tokens → Generate new token (classic) →
tick `repo`. Or use the GitHub CLI: `gh auth login` then push.

## 2. Connect the repo to Vercel

1. https://vercel.com/stepskas-2556s-projects/munchies-campaign-emails/settings/git
2. **Connect Git Repository** → pick `oneqwerty1-design/munchies-emails`
3. Leave build settings empty — static site, no build step

Done. Every push to `main` deploys to https://munchies-campaign-emails.vercel.app

## Then what

Claude edits `index.html` / `styles.css`, commits, pushes. Vercel handles the rest.
No more re-uploading the whole file tree through the API.

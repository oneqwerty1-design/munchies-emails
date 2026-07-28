# One-time setup — connect this repo to Vercel

The repo is initialised and committed on `main`. Two steps and deploys become automatic.

## 1. Push to GitHub

Create an empty repo at https://github.com/new — name it `munchies-campaign-emails`,
**don't** add a README or .gitignore (this repo already has them).

Then, from inside this folder:

```bash
git remote add origin https://github.com/YOUR-USERNAME/munchies-campaign-emails.git
git push -u origin main
```

## 2. Connect it to the existing Vercel project

1. Go to https://vercel.com/stepskas-2556s-projects/munchies-campaign-emails/settings/git
2. Click **Connect Git Repository**
3. Pick `munchies-campaign-emails`
4. Leave build settings empty — it's static, no build step

Done. Every push to `main` deploys to https://munchies-campaign-emails.vercel.app

## After that

Claude edits `index.html` / `styles.css` directly and commits. No more hand-copying
file contents through the API, which is what broke the retention page on Jul 28.

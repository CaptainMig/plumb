# Plumb · Media Audit System
**Three-layer buyside audit. Structurally independent verdict.**
AC Ads · v3 · 2026

---

## Files

| File | URL | Description |
|------|-----|-------------|
| `index.html` | `/` | Main prototype — pitch deck + four working tools |
| `pipeline.html` | `/pipeline` | Data pipeline architecture diagram |
| `vercel.json` | — | Routing config |

---

## Deploy to Vercel

### First time

```bash
# 1. Install Vercel CLI if not already installed
npm install -g vercel

# 2. From this directory
vercel

# Follow the prompts:
#   Set up and deploy? Yes
#   Which scope? (your account)
#   Link to existing project? No
#   Project name: plumb (or plumb-acads)
#   In which directory is your code? ./
#   Want to override settings? No

# Vercel will output your live URL.
```

### Subsequent deploys (after edits)

```bash
vercel --prod
```

That's it. No build step. No dependencies. Static HTML.

---

## Deploy to Vercel via GitHub (recommended)

1. Create a new repo on GitHub named `plumb`
2. From this directory:

```bash
git init
git add .
git commit -m "Plumb v3 — initial deploy"
git remote add origin https://github.com/YOUR_USERNAME/plumb.git
git push -u origin main
```

3. Go to [vercel.com](https://vercel.com) → **Add New Project** → import the `plumb` repo
4. Framework preset: **Other**
5. Build command: *(leave blank)*
6. Output directory: *(leave blank or `.`)*
7. Click **Deploy**

Every subsequent `git push` to `main` auto-deploys.

---

## URLs after deploy

```
yourdomain.vercel.app/           → Main prototype
yourdomain.vercel.app/pipeline   → Pipeline architecture
```

To use a custom domain (e.g. `plumb.acads.com`):
Vercel Dashboard → your project → Settings → Domains → Add domain.

---

## Editing

Both files are single-file HTML — no framework, no npm, no build step.
Edit `index.html` or `pipeline.html` directly, then redeploy with `vercel --prod`
or push to GitHub if connected.

---

## What the 47 / sample data means

The audit counts and dollar figures in the History tool are **illustrative**.
They show what the calibration record looks like once real audits accumulate.
Replace with real numbers as closed audits are logged.

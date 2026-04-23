# International Wood — Buyers Guide 2025 (Private Preview)

Password-gated web preview of the Buyers Guide 2025 issue of *International
Wood Magazine*, rebuilt from the source flipbook as a set of linkable,
SEO-friendly pages.

Visitors enter the password once; the browser remembers them for 30 days so
they can navigate every feature, advertiser, and directory page freely.

## Hosting on GitHub Pages

1. Create a new repository on GitHub (public is fine — HTML is encrypted).
2. Push this folder:
   ```sh
   git init
   git add .
   git commit -m "Initial preview build"
   git remote add origin https://github.com/<you>/<repo>.git
   git branch -M main
   git push -u origin main
   ```
3. In the repository's **Settings → Pages**, set Source to `main` / `/ (root)`.
4. GitHub publishes to `https://<you>.github.io/<repo>/`.

## Sharing the link

Share out-of-band (Slack DM, email, etc.):
- URL: `https://<you>.github.io/<repo>/`
- Password: (what you chose when running `publish.py`)

## Rebuilding

Rerun `python3 scraper/publish.py [password]` to regenerate after content or
design changes.

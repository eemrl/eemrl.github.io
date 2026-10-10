# lauren-mee.com

Static portfolio site for Lauren Mee, hosted on GitHub Pages. No build step.

## Files
- `index.html` — the whole site
- `CNAME` — tells GitHub Pages to serve at lauren-mee.com
- `.nojekyll` — skips Jekyll processing

## Before publishing
1. Confirm her credited title on Marvel's Wolverine (currently "Writer").
2. Confirm the Batman: The Enemy Within WGA nomination line.

## Deploy
1. Push these files to the root of the repo's default branch.
2. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Custom domain: `lauren-mee.com` (GitHub fills this in from `CNAME`), then tick "Enforce HTTPS" once the certificate is issued.

## DNS (at the domain registrar — the domain currently points at Weebly)
- `www` → CNAME → `eemrl.github.io`
- Apex `lauren-mee.com` → A records:
  185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

Remove the old Weebly records first. With both set, GitHub redirects www to lauren-mee.com. DNS can take up to 24 hours to settle. Cancel the Weebly plan only after the GitHub version is live.

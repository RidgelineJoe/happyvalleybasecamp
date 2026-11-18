# Happy Valley Basecamp — happyvalleybasecamp.com

Static one-page site for the 3775 N Atherton rental, hosted free on GitHub Pages.

## Files

- `index.html` — the whole site
- `CNAME` — tells GitHub Pages to serve on happyvalleybasecamp.com
- `images/` — photos (create this folder; file names below)

## Photos (images/ folder)

Already sized, renamed, and stripped of phone location data. To swap one (e.g. a snow hero shot), save the new photo with the same file name and upload it over the old one.

| File | Shot |
|---|---|
| hero.jpg | Acreage with the house in the distance. Swap seasonally. |
| exterior.jpg | Front of the farmhouse |
| land.jpg | Back yard and lawn |
| porch.jpg | Front porch |
| kitchen.jpg / kitchen-2.jpg | Kitchen |
| living.jpg | Living area |
| dining.jpg | Dining area |
| bedroom-1.jpg / bedroom-2.jpg | Queen bedrooms |
| bedroom-3.jpg | Twin bedroom |
| bathroom.jpg | Bathroom |
| workspace.jpg | Sit/stand desk |

## Deploy (one time)

1. In the RBS GitHub account, create a new **public** repository named `happyvalleybasecamp`.
2. Upload `index.html`, `CNAME`, `README.md`, and the `images/` folder.
3. Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.
4. Settings → Pages → Custom domain: `happyvalleybasecamp.com` → Save.
5. At the domain registrar, add DNS records:
   - Four `A` records for `@` pointing to: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record for `www` pointing to: `<your-github-username>.github.io`
6. Wait for DNS to propagate (minutes to a few hours), then check **Enforce HTTPS** in Settings → Pages.

## Updating

Edit the file or swap a photo in the repo; the site republishes on its own within a minute or two.

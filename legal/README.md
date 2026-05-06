# BetMate — Legal pages

Static HTML pages for the App's Privacy Policy and Terms of Use. Designed
to be hosted for free on **GitHub Pages**, then linked from the Google
Play / App Store listings (Privacy Policy URL is mandatory on Play Store).

## Files

| File | Purpose |
|------|---------|
| `index.html` | Landing page with links to both documents |
| `privacy.html` | Privacy Policy (data, AdMob, third-party, contact) |
| `terms.html`   | Terms of Use (informational only, no liability, age 18+) |
| `style.css`    | Shared dark-theme stylesheet matching the app |

Effective date in each file is set automatically to the current day on
page load.

## How to publish on GitHub Pages (free, ~5 minutes)

### Option A — Dedicated repo

1. Create a new GitHub repo, e.g. `betmate-legal` (public).
2. Copy the contents of this `legal/` folder into the repo root.
3. Push to `main`.
4. In the repo on GitHub, open **Settings → Pages**.
5. Under **Source**, pick **Deploy from a branch** → branch `main` → folder
   `/ (root)` → **Save**.
6. Wait ~30s. GitHub will publish the site at:
   `https://<your-github-username>.github.io/betmate-legal/`

### Option B — User/organization site

If you already have `https://<username>.github.io`, drop the `legal/`
folder there and you'll get
`https://<username>.github.io/legal/privacy.html` etc.

### Custom domain (optional)

If you own a domain like `betmate.app`, add it under
**Settings → Pages → Custom domain** and create a `CNAME` DNS record
pointing to `<username>.github.io`.

## Where to put the URLs

After publishing, copy the URLs and use them in:

- **Google Play Console** → App content → Privacy policy → paste the
  Privacy Policy URL.
- **App Store Connect** → App Information → Privacy Policy URL.
- **AdMob** → app settings → Privacy Policy URL.
- Optionally: link to the `terms.html` page from the in-app
  `TermsView` (e.g. add a "View online" button).

# Color Fun – legal & support site (GitHub Pages)

Static site with Privacy Policy, Terms of Use and Support pages in English (root) and Turkish (`/tr`). No build step, no tracking, no cookies.

## Contact

The support address used on all pages is **elappstest@gmail.com**. To change it, replace it in all six pages.

## Publish on GitHub Pages

Option A — separate repository (simplest):
```bash
cd legal-site
git init && git add . && git commit -m "Legal site"
git branch -M main
git remote add origin git@github.com:<your-user>/colorfun-legal.git
git push -u origin main
```
GitHub → repo → Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)` → Save.

Your URLs will be:

| Page | URL |
|---|---|
| Home | `https://<your-user>.github.io/colorfun-legal/` |
| Privacy Policy (EN) | `https://<your-user>.github.io/colorfun-legal/privacy.html` |
| Terms of Use (EN) | `https://<your-user>.github.io/colorfun-legal/terms.html` |
| Support (EN) | `https://<your-user>.github.io/colorfun-legal/support.html` |
| Gizlilik (TR) | `https://<your-user>.github.io/colorfun-legal/tr/gizlilik.html` |
| Koşullar (TR) | `https://<your-user>.github.io/colorfun-legal/tr/kosullar.html` |
| Destek (TR) | `https://<your-user>.github.io/colorfun-legal/tr/destek.html` |

## Where the URLs go

- App: `.env.local` (and EAS environment variables) → `EXPO_PUBLIC_PRIVACY_URL`, `EXPO_PUBLIC_TERMS_URL` (shown in the parent paywall).
- App Store Connect: Privacy Policy URL, Support URL; add the Terms URL to the description (or use Apple's standard EULA).
- Google Play Console: Privacy policy URL (App content), website/email in store listing.

# Dot Clash — Legal site (Jekyll)

Static legal pages for Dot Clash. Published at **https://vividmemories-games.github.io** via GitHub Pages (this repo).

## Setup

1. Edit **`_data/legal.yml`** — entity name, email, address, dates, `personalized_ads`, etc.
2. Install Ruby, then:

```bash
bundle install
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000).

## GitHub Pages

This repo is a **user/org site** (`vividmemories-games.github.io`). Jekyll source is the **repo root** (not `/docs`).

1. Repo → **Settings** → **Pages** → **Build and deployment**
2. **Source:** GitHub Actions (uses `.github/workflows/pages.yml`)
3. Push to `main` — the workflow builds and deploys

If you previously used **Deploy from branch → `/docs`**, switch to **GitHub Actions** or set the folder to **`/ (root)`**. The `/docs` setting causes `style.scss` / missing-directory build failures because this site has no `docs/` folder.

Published URLs (with `permalink: pretty`):

| Page | Path |
|------|------|
| Index | `/` |
| Privacy Policy | `/privacy-policy/` |
| Terms | `/terms-and-conditions/` |
| EULA | `/eula/` |
| Cookie Policy | `/cookie-policy/` |
| Contact Us | `/contact/` |
| Delete Your Data | `/delete-data/` |
| Privacy Choices | `/privacy-choices/` |

Use the **Privacy Policy** URL in AdMob UMP and store privacy forms. Use **Delete Your Data** and **Contact** URLs in App Store / Play Console compliance fields.

## Files

| Path | Purpose |
|------|---------|
| `_data/legal.yml` | Shared placeholders (edit once) |
| `privacy-policy.md` | AdMob / store privacy URL |
| `terms-and-conditions.md` | Terms of service |
| `eula.md` | Optional license |
| `cookie-policy.md` | Website cookies only |
| `contact.md` | Support (in-app form primary) |
| `delete-data.md` | In-app deletion instructions |
| `privacy-choices.md` | Ad consent / privacy choices |

## Dot Clash app repo

The Flutter app lives in a separate repo (`Dot_Clash`). Legal URL constants in `lib/core/env/app_env.dart` must match this site.

## Personalized ads

In `_data/legal.yml`, set `personalized_ads: true` only if AdMob serves personalized ads (requires iOS ATT). The Privacy Policy body switches automatically.

## Not legal advice

Review all pages with qualified counsel before publishing.

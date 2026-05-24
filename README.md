# Dot Clash — Legal site (Jekyll)

Static legal pages for Dot Clash (Privacy Policy, Terms, EULA, Cookie Policy). Host on **GitHub Pages**, Netlify, or any static host.

## Setup

1. Edit **`_data/legal.yml`** — entity name, email, address, dates, `personalized_ads`, etc.
2. Install Ruby, then:

```bash
cd docs
bundle install
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000).

## GitHub Pages

1. Repo → **Settings** → **Pages** → Source: **Deploy from branch**
2. Branch: `main` (or your default), folder: **`/docs`**
3. Set `url` and `baseurl` in `_config.yml` if using a project site (`https://user.github.io/RepoName/`)

Published URLs (with `permalink: pretty`):

| Page | Path |
|------|------|
| Index | `/` |
| Privacy Policy | `/privacy-policy/` |
| Terms | `/terms-and-conditions/` |
| EULA | `/eula/` |
| Cookie Policy | `/cookie-policy/` |

Use the **Privacy Policy** URL in AdMob UMP (plan A3) and store privacy forms.

## Files

| Path | Purpose |
|------|---------|
| `_data/legal.yml` | Shared placeholders (edit once) |
| `privacy-policy.md` | AdMob / store privacy URL |
| `terms-and-conditions.md` | Terms of service |
| `eula.md` | Optional license |
| `cookie-policy.md` | Website cookies only |
| `legal/` | Legacy Word export + combined markdown |

## Personalized ads

In `_data/legal.yml`, set `personalized_ads: true` only if AdMob serves personalized ads (requires iOS ATT). The Privacy Policy body switches automatically.

## Not legal advice

Review all pages with qualified counsel before publishing.

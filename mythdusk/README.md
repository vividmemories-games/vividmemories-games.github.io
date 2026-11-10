# MythDusk — Legal site (Jekyll)

Static legal + store compliance pages for **MythDusk**. Lives in this org site under **`/mythdusk/`**.

Published at **https://vividmemories-games.github.io/mythdusk/**.

## Setup

1. Edit **`_data/legal.yml`** — entity name, email, address, dates, `personalized_ads`, etc.
2. Edit **`_data/app.yml`** — App Store / Play Store URLs when listings are live.
3. Install Ruby, then:

```bash
bundle install
bundle exec jekyll serve --baseurl /mythdusk
```

Open [http://localhost:4000/mythdusk/](http://localhost:4000/mythdusk/).

`_config.yml` sets:

- `url: "https://vividmemories-games.github.io"`
- `baseurl: "/mythdusk"`

## Published URLs

| Page | Path |
|------|------|
| Index | `/mythdusk/` |
| Privacy Policy | `/mythdusk/privacy-policy/` |
| Terms | `/mythdusk/terms-and-conditions/` |
| EULA | `/mythdusk/eula/` |
| Cookie Policy | `/mythdusk/cookie-policy/` |
| Contact Us | `/mythdusk/contact/` |
| Delete Your Data | `/mythdusk/delete-data/` |
| Privacy Choices | `/mythdusk/privacy-choices/` |
| Download | `/mythdusk/download/` |

Hardcode these paths in the Flutter app (privacy, delete-data, contact, terms). Share **`/mythdusk/download/`** as the store landing page.

## Files

| Path | Purpose |
|------|---------|
| `_data/legal.yml` | Shared placeholders (edit once) |
| `_data/app.yml` | App Store / Play Store URLs |
| `assets/css/main.css` | Shared legal-site styles |
| `assets/images/` | App icon, store badges |
| `download/index.html` | Marketing download landing page |
| `privacy-policy.md` | AdMob / store privacy URL |
| `terms-and-conditions.md` | Terms of service |
| `eula.md` | Optional license |
| `cookie-policy.md` | Website cookies only |
| `contact.md` | Support |
| `delete-data.md` | Account deletion instructions |
| `privacy-choices.md` | Ad consent / privacy choices |

## Soft-launch ads flag

In `_data/legal.yml`:

- Set `ads_enabled: true` only when AdMob ships in a live build. Soft launch defaults to `false` so privacy/terms copy stays honest.
- Set `personalized_ads: true` only if AdMob serves personalized ads (requires iOS ATT). Default is `false`.


## Not legal advice

Draft policies for compliance scaffolding. Review with qualified counsel before publishing.

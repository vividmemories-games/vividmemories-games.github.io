# vividmemories-games.github.io

Org GitHub Pages site for Vivid Memories Games apps.

| App | Path |
|-----|------|
| **Dot Clash** | `/` (site root) |
| **MythDusk** | `/mythdusk/` |

## Local preview

### Dot Clash (root)

```bash
bundle install
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000).

### MythDusk

```bash
cd mythdusk
bundle install
bundle exec jekyll serve --baseurl /mythdusk
```

Open [http://localhost:4000/mythdusk/](http://localhost:4000/mythdusk/).

## Deploy

Push to `main`. `.github/workflows/pages.yml` builds Dot Clash into `_site/` and MythDusk into `_site/mythdusk/`, then deploys both.

Keep these at the **domain root** (Dot Clash / platform requirements):

- `app-ads.txt`
- `.well-known/` (e.g. Android App Links)
- `apple-app-site-association`

## Dot Clash URLs

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
| Download | `/download/` |

Edit `_data/legal.yml` and `_data/app.yml`.

## MythDusk URLs

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

Edit `mythdusk/_data/legal.yml` and `mythdusk/_data/app.yml`.

## Not legal advice

Review all pages with qualified counsel before publishing.

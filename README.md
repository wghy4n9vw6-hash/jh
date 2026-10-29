# Medhane Hagos Mesgena, MD — search presence kit

Owned-property hub and working files for building search-engine presence around the name
**Medhane Hagos Mesgena** and the article site
https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/.

| Path | What it is |
|---|---|
| `index.html` | Entity hub page (bio, publications, profile links, schema.org `Person` JSON-LD). Serve it with GitHub Pages. |
| `sitemap.xml`, `robots.txt` | For the GitHub Pages hub. |
| `docs/reputation-seo-plan.md` | The prioritized action plan, with the baseline audit of what search engines show today. |
| `docs/article-seo-template.md` | Checklist and front-matter template for every new article on the site. |
| `articles/` | Companion article drafts (same format as the peptide-compounding piece) ready for physician review and publishing. |
| `articles/content-calendar.md` | Next 12 article topics with target queries. |

## Enabling the hub page

GitHub → repository **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick this
branch and the `/ (root)` folder. The page then serves at `https://wghy4n9vw6-hash.github.io/jh/`.
If a custom domain is pointed at it later, update the URLs in `index.html`, `sitemap.xml` and `robots.txt`.

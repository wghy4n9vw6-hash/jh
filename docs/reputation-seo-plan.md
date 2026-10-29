# Search presence plan — Medhane Hagos Mesgena, MD

Goal: when someone searches **Medhane Hagos Mesgena**, **Medhane Mesgena** or **Dr. Medhane Mesgena**, the first page is
dominated by properties you own or control and by publications that carry your byline, led by the article site
https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/.

Prepared 2026-10-29 from live search results. The site itself could not be fetched from this environment, so items
marked **[verify on site]** need a two-minute check in your browser.

---

## 1. Baseline: what search engines show today

Query `"Medhane Hagos Mesgena"` (Google-backed results, 2026-10-29):

| # | Result | Control |
|---|---|---|
| 1 | WebMD physician directory listing | Claimable |
| 2 | OCNJ Daily — "Early Detection, Prevention & Health Screenings" (Dec 26, 2025) | Your byline |
| 3 | North Penn Now — "Designing Healthcare That Reaches Communities Before Crisis" (Feb 24, 2026) | Your byline |
| 4 | OCNJ Daily — "Building Global Readiness into U.S. Healthcare Training" (Oct 31, 2025) | Your byline |
| 5 | NZ Doctor — tribunal censure article naming a Napier GP "Medhane Mesgena" | Not controllable |
| 6 | drmedhanemesgena.com | Yours |
| 7 | drmedhanehagosmesgena.com | Yours |
| 8 | medhanemesgena.com — CME article | Yours |

Also surfaced on related queries: Doximity, U.S. News Health, MD.com, ZoomInfo.

Query `site:medhane-hagos-mesgena.rainymoon131.chatgpt.site`: **zero results.** The article site is not indexed at all.
That is the single biggest problem and the first thing to fix. Nothing else in this plan helps the article site
until a crawler can see it.

Two structural weaknesses:

- **The article site has no authority.** It is a sub-sub-domain on a third-party platform with no inbound links, no
  history and no verified ownership in Search Console. Search engines treat it as brand new and unimportant.
- **Your presence is fragmented across four sites** with near-identical bios. Four thin sites split link equity
  four ways and can look like a network of duplicates. One strong site beats four weak ones.

## 2. Priority actions, in order

### P0 — Get the article site crawlable and indexed (this week)

1. **Confirm the site is published publicly** in ChatGPT Sites (Share → "Anyone with the link" / public), not
   "Only you". OpenAI's help pages say only public Sites are reachable without login. **[verify on site]**
2. **Check for a noindex.** Open the article page, view source, search for `noindex` and look at the response headers
   for `X-Robots-Tag`. Also open `/robots.txt` on the site. If the platform blocks crawlers you must move the content
   (see P1). **[verify on site]**
3. **Verify ownership in Google Search Console** as a URL-prefix property for
   `https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/`. Use the HTML-tag method if Sites lets you add a
   `<meta>` to the head, otherwise the HTML-file method. If neither is possible on the platform, that is a strong
   reason to move to a custom domain, where DNS verification always works.
4. **Submit the sitemap** (`/sitemap.xml`) in Search Console, then use URL Inspection → **Request indexing** on the
   homepage and on every article URL. Repeat Request indexing for each new article the day it goes live.
5. **Verify in Bing Webmaster Tools** (import from Search Console with one click) and submit the same sitemap.
   Bing's index feeds ChatGPT search, Copilot and DuckDuckGo, so this covers AI answer engines as well.
6. **Create inbound links today** from properties you already control so crawlers discover the site without waiting:
   - Add a "Latest articles" link in the header or footer of all three personal sites pointing at the article site.
   - Link to it from your Doximity, WebMD, U.S. News, MD.com and LinkedIn profiles (website field).
   - Publish the GitHub Pages hub in this repository (`index.html`), which links to it with Person schema.
   - Post each new article on LinkedIn with the link.

### P1 — Move to a custom domain and consolidate (next 2–4 weeks)

7. **Put the article site on a domain you own.** ChatGPT Sites supports connecting a domain you control via DNS
   (owner-only setting). Recommended: `articles.drmedhanehagosmesgena.com` or, better, publish the articles directly
   under `drmedhanehagosmesgena.com/articles/`. Reasons: authority accrues to a domain you keep forever, DNS
   verification in Search Console becomes trivial, and you are insulated if the platform changes its URL scheme.
   After moving, 301-redirect or at least re-link every old URL and resubmit the sitemap.
8. **Pick one primary site and fold the others into it.** `drmedhanehagosmesgena.com` carries your full name and
   already has an article; make it primary. Keep `drmedhanemesgena.com` and `medhanemesgena.com` registered but
   301-redirect them to the primary. If you prefer to keep them live, give each a distinct purpose (one = practice,
   one = speaking/media kit) and distinct copy so they are not duplicates.

### P2 — Make every property say the same thing about the same person (entity consistency)

9. Use the **exact same name string** everywhere: `Medhane Hagos Mesgena, MD`. Put it in the `<title>`, the H1 of
   the About page, the author byline on every article and the author schema. Search engines merge mentions into one
   entity only when the signals agree.
10. Add **`Person` JSON-LD with `sameAs`** to the primary site (copy the block from `index.html` in this repo and
    change the `url`/`@id`). List every profile and site in `sameAs`. Add `Article` JSON-LD with `author` →
    that Person on every article page. **[verify on site: whether Sites allows custom head markup]**
11. Use one identical **professional headshot** and one identical **short bio** (two sentences) on every profile and
    site. Image search and Knowledge Panel generation key off repeated images.
12. **Claim and complete** every directory that already ranks: WebMD, Doximity, U.S. News Health, MD.com. Fill the
    website field, bio, photo and specialty. Each claimed profile is a page-one slot you control.
13. **Create the profiles that are missing and rank well for names**: LinkedIn (public profile, custom URL
    `/in/medhanehagosmesgena`, publish articles there too), Healthgrades, Vitals, Google Business Profile (if you see
    patients at a fixed location), a YouTube channel (even three short explainer videos), Muck Rack (journalist-facing
    author page), and an author page on Medium or Substack that republishes with a canonical link to the original.

### P3 — Publish steadily, in the same format that already works (ongoing)

The peptide-compounding article is the right model: a dated, sourced reaction to a health-policy or clinical news event,
written for patients and colleagues from a family-medicine perspective. Timely pieces earn fresh-content boosts and
pick up long-tail queries that nobody else owns yet.

14. **Cadence:** two articles per week minimum for the first 90 days, then one per week. Publish within 48 hours of the
    news event. Three drafts in `articles/` are ready for your review; `articles/content-calendar.md` has twelve more
    topics.
15. **Every article follows `docs/article-seo-template.md`**: name in the byline, a one-paragraph author box linking to
    the hub, a specific title that includes the news entity (e.g. "BPC-157", "Medicare Part D 2027"), two to four
    internal links to your other articles, and three to six outbound links to primary sources (HHS, FDA, CMS, CDC).
16. **Build topic clusters.** Group articles by theme (peptides and compounding; vaccines and respiratory season;
    Medicare costs; preventive screening; health equity and access). Interlink within clusters. Clusters are how a
    small site ranks for topics, not just for your name.
17. **Syndicate** each piece to LinkedIn Articles 24 hours after it goes live, with a link back and a line saying
    "Originally published at …". Post a short thread or summary on X/Threads with the link.

### P4 — Earned coverage under your byline (ongoing)

18. Keep placing contributed pieces in regional outlets like OCNJ Daily and North Penn Now; they already rank on page
    one for your name. Pitch the same editors with the companion drafts. Where a placement is paid, let the outlet label
    it as sponsored; mislabeled paid content can be devalued.
19. Register as an expert source on **Qwoted, Featured (formerly Terkel) and Help a B2B Writer**. Answer two queries
    a week on primary care, preventive care, peptides/GLP-1 compounding, Medicare and vaccines. Each quote is an
    independent page carrying your name.
20. Pitch three to five **podcast interviews** on health equity or rural access. Show-notes pages are durable,
    well-linked results.
21. Ask institutions you work with (clinics, VES/C&P programs, medical schools, nonprofits) to publish a short profile
    or news item with your full name and a link to the primary site.

## 3. The NZ Doctor result

A tribunal article from NZ Doctor naming a Napier GP "Medhane Mesgena" currently sits around position 5 for your name.
It cannot be removed by SEO, and nothing in this plan should attempt to attack or suppress it directly. The legitimate
and effective approach is the one above: more authoritative, fresher, more relevant results that carry your name and
earn clicks. Historically, eight to ten strong owned and earned results push a single older news item to page two
within three to six months of consistent publishing. If it is you and you want to address it, a factual, brief note on
your About page is your call; do not reference it anywhere else.

## 4. What not to do

- No duplicate or near-duplicate sites, doorway pages or scraped content. Consolidate instead (P1).
- No fake reviews, purchased links, private blog networks or automated link submissions.
- No keyword stuffing of your name; natural bylines and author boxes are enough.
- No AI-generated medical articles published without your review. Every piece carries your medical credibility; the
  drafts in `articles/` are starting points for you to edit, not finished copy.

## 5. Measure monthly

- Search Console: impressions and clicks for the queries `medhane hagos mesgena`, `medhane mesgena`,
  `dr medhane mesgena`; indexed-page count for the article site.
- Manual check in an incognito window: screenshot the first 20 results for the three name queries on Google and Bing
  on the first of each month. Count how many are yours.
- Target by end of month 3: article site indexed with every article; 7 of the top 10 for the full-name query
  owned or bylined. Target by month 6: 9 of 10.

## 6. Sitemap checklist for the article site **[verify on site]**

The sitemap at `/sitemap.xml` should:

- be valid XML in the `http://www.sitemaps.org/schemas/sitemap/0.9` namespace;
- list every public article URL with the exact canonical form (same scheme, host, trailing-slash convention);
- include `<lastmod>` in `YYYY-MM-DD` form and update it when an article changes;
- return HTTP 200 with content-type `application/xml` or `text/xml`;
- be referenced by a `Sitemap:` line in `/robots.txt`;
- contain only URLs that return 200 and are not marked noindex.

If any of those fail and the platform does not let you fix them, that is one more reason to move to the custom domain.

# gkoumasd.github.io

Personal site of Dimitris Gkoumas.

| File | Purpose |
|---|---|
| `index.html` | About me (home page) |
| `ai-under-the-hood.html` | AI Under the Hood: the handbook |
| `sitemap.xml` | Lists both pages for search engines |
| `robots.txt` | Allows crawling and points to the sitemap |
| `assets/og/og-home.png`, `assets/og/og-notes.png` | Preview images shown when a link is shared (LinkedIn, X, Slack) |
| `assets/images/square.jpg` | Profile photo, already in the repository |

## Publish on GitHub Pages

1. Copy these files into the root of the `gkoumasd.github.io` repository, replacing the old `index.html`. Keep the existing `assets/images/` folder for the photo.
2. Commit and push to the default branch:
   ```bash
   git add index.html ai-under-the-hood.html sitemap.xml robots.txt assets/og README.md
   git commit -m "Add SEO tags, sitemap and preview images"
   git push
   ```
3. The site updates at https://gkoumasd.github.io/ within a minute or two.

Both pages are self-contained HTML. They load Google Fonts and KaTeX (for equations) from public CDNs, and need no build step.

## Get found on Google (one-time)

1. Open [Google Search Console](https://search.google.com/search-console), add a **URL prefix** property for `https://gkoumasd.github.io/`, and verify it. The HTML-tag method gives a `<meta name="google-site-verification" ...>` line to paste into the `<head>` of `index.html`.
2. In **Sitemaps**, submit `sitemap.xml`.
3. In **URL inspection**, request indexing for both pages.
4. Add the site link to LinkedIn, your Google Scholar profile and your GitHub profile.

When you change a page, update its `<lastmod>` date in `sitemap.xml`.

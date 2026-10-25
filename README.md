# Search & AI Discovery Desk

A standalone, responsive single-page guide for preparing a website URL for search-engine discovery and understanding how AI-powered search products find public pages. The entire interface lives in [`index.html`](index.html); it has no build step, backend, account integration, or runtime dependency.

## What the page does

- **Prepare a page URL:** accepts an HTTP(S) URL, adds `https://` if the scheme is omitted, removes the fragment, and keeps query parameters. It then provides copy buttons for the page URL and the site's conventional `/sitemap.xml` address.
- **Open official submission tools:** links to Google Search Console, Bing Webmaster Tools, Brave's URL submission form, Yandex Webmaster, Baidu's link-submission tool, and Naver Search Advisor. Notes explain when sign-in, ownership verification, or regional knowledge is likely needed.
- **Offer an optional IndexNow ping:** after the site owner provides a key already published on the same site, the page opens the official IndexNow endpoint for the prepared URL. The page does not store the key or claim that the URL was indexed; check the endpoint's response.
- **Explain AI-search discovery:** summarizes the documented crawler/discovery routes for ChatGPT Search, Google's AI features, Microsoft Copilot, Perplexity, Claude Search, DuckDuckGo/DuckAssist, Apple search experiences, and other answer engines. It distinguishes search crawlers from model-training crawlers; training permissions remain a separate site-owner choice.
- **Generate a robots.txt suggestion:** creates a copyable snippet for selected search crawlers and a site-specific sitemap line. Review it against existing rules before use, and keep private paths disallowed.
- **Provide a readiness checklist:** highlights public crawl access, accidental `noindex` blocks, XML sitemaps, useful crawlable content, accurate structured data, and genuine independent references.

## What it does not do

This is a client-side guide, not an indexing service. It never signs in to webmaster accounts, sends submissions on the visitor's behalf to search-console forms, stores credentials, or promises indexing, rankings, or AI citations. Search submission is a request or hint; providers decide whether and when to crawl or index. For IndexNow, the visitor must own the site and publish the matching verification key before sending a ping.

## Run or host it

Open `index.html` directly or serve it from any static hosting provider. No compilation or package installation is required. If hosting on GitHub Pages, publish the repository's root directory as a static site. Use the public canonical URL of your own site in the page field; the repository does not include a site-specific sitemap or `robots.txt` because the final hosting domain is chosen by the site owner.

## Sources

The page links to primary provider documentation and submission tools. A fuller reference list and maintenance notes are in [`docs/indexing-desk.md`](docs/indexing-desk.md). Provider interfaces and crawler policies can change; verify the linked official documentation before relying on a route.

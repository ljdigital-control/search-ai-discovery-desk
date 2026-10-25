# Indexing Desk: source and behavior notes

The standalone page is [`../index.html`](../index.html). It is a static HTML/CSS/JavaScript file with no runtime dependencies. Its deployment hostname is not hard-coded; visitors enter the public URL they want to prepare.

## URL preparation and submission routes

The URL helper accepts HTTP and HTTPS URLs, adds HTTPS when no scheme is supplied, removes fragments, and preserves query parameters. It derives a conventional `/sitemap.xml` URL from the submitted page's origin and creates a site-specific `robots.txt` suggestion. The page includes official portals or instructions for Google Search Console, Bing Webmaster Tools, Brave Search, Yandex Webmaster, Baidu Search Resource Platform, and Naver Search Advisor. These services may require sign-in, verified ownership, or a region-specific account.

The optional IndexNow form requires a key that the visitor has already published on the same site. A custom key-file URL must share the submitted page's origin. The page opens the official IndexNow endpoint in a new tab; the visitor checks its response. It does not persist the key or represent the response as proof of indexing.

## AI search guidance

The page explains the currently documented discovery/crawler routes for ChatGPT Search, Google AI Overviews and AI Mode, Microsoft Copilot, Perplexity, Claude Search, DuckDuckGo and DuckAssist, Apple search experiences, and other answer engines. It notes that there is no universal AI URL-submit portal and distinguishes search crawlers from model-training crawlers. Its optional `robots.txt` snippet intentionally excludes training crawlers; visitors should review existing rules and retain restrictions on private paths.

## Sources checked

Provider-owned documentation and tools used for the page:

- [Google Search Console](https://search.google.com/search-console/welcome), [Google recrawl guidance](https://developers.google.com/search/docs/crawling-indexing/ask-google-to-recrawl), [Google sitemap requirements](https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap), and [Google AI features](https://developers.google.com/search/docs/appearance/ai-features)
- [Bing Webmaster Tools](https://www.bing.com/webmasters/about), [Bing URL submission](https://www2.bing.com/webmasters/help/URL-Submission-62f2860b), and [Bing IndexNow setup](https://www2.bing.com/indexnow/getstarted)
- [IndexNow protocol and key requirements](https://www.indexnow.org/documentation) and [current participating engines](https://www.indexnow.org/searchengines)
- [Brave URL submission](https://search.brave.com/submit-url) and [Brave crawler guidance](https://search.brave.com/help/brave-search-crawler)
- [Yandex Webmaster](https://webmaster.yandex.com/), [Yandex sitemap guidance](https://yandex.com/support/webmaster/en/indexing-options/sitemap), and [Yandex recrawl guidance](https://yandex.com/support/webmaster/en/robot-workings/new-changed)
- [Baidu link submission](https://ziyuan.baidu.com/linksubmit/url) and [Naver Search Advisor sitemap/RSS guidance](https://searchadvisor.naver.com/guide/request-feed)
- [OpenAI crawler guide](https://developers.openai.com/api/docs/bots), [Perplexity crawler policy](https://docs.perplexity.ai/docs/resources/perplexity-crawlers), [Anthropic crawler policy](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler), [Applebot](https://support.apple.com/en-us/119829), and [DuckAssistBot](https://duckduckgo.com/duckduckgo-help-pages/results/duckassistbot)

These links and product behavior may change. Confirm live provider documentation before relying on a submission route. No single service offers a public URL-submit endpoint for every AI assistant, and no listing technique guarantees ranking or citation.

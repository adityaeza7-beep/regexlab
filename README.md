# RegexLab

**Free, browser-only regex tester built for Google Analytics 4** — live at [regextester.site](https://regextester.site/).

No server, no accounts, no data leaves your browser: 100% client-side JavaScript RegExp.

## Why GA4 regex is different

- GA4 filters **full-match** by default — wrap substring patterns in `.*`
- GA4 runs **RE2** (like BigQuery, Go and Rust): no lookahead, no lookbehind, no backreferences

## What's inside

- **[Live regex tester](https://regextester.site/)** — match/no-match per line, flags, substitution
- **[Regex pattern library](https://regextester.site/regex-patterns/)** — 17 tested patterns (dates, emails, URLs, IPs, UUIDs, UTM parameters, log levels) with copy-paste snippets for JS / Python / SQL / BigQuery
- **GA4 guides** — [cheat sheet](https://regextester.site/ga4-regex-cheatsheet/), [page path regex](https://regextester.site/ga4-page-path-regex/), [event filter regex](https://regextester.site/ga4-event-filter-regex/), [match types](https://regextester.site/ga4-regex-match-types/), [custom channel grouping](https://regextester.site/ga4-custom-channel-grouping-regex/)
- **[RE2 vs PCRE](https://regextester.site/re2-vs-pcre/)** — every unsupported construct with its working replacement

## Quick examples

```
# GA4 page path filter (full-match semantics)
.*/blog/.*

# GA4 ecommerce event filter
(view_item|add_to_cart|begin_checkout|add_payment_info|purchase)
```

Free to use. Built for analysts who got tired of pasting patterns into GA4 blindly.

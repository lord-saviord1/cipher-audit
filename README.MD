# CIPHER::AUDIT

**Schema & Search Visibility Console** by [Cipher PR](https://cipherpr.me)

A zero-dependency, single-file web console for client-side SEO checks. Open `index.html` and go.

[Live demo](https://lord-saviord1.github.io/cipher-audit/) · [Agent skill on Agensi](https://agensi.io/skills/cipher-audit) · MIT licensed

<!-- Add a screenshot or short demo GIF: ![CIPHER::AUDIT screenshot](docs/screenshot.png) -->

## What it does
- **Schema audit:** parses `<script type="application/ld+json">` blocks or raw JSON-LD, checks required and recommended properties for Person, Organization, WebSite, WebPage, Article, BlogPosting, BreadcrumbList, JobPosting, CreativeWork and ProfilePage, and scores each entity.
- **Search visibility:** drop in a Google Search Console Queries or Pages CSV to get total clicks and impressions, blended CTR, impression-weighted position, top rows, and high-impression low-CTR opportunities.
- **Optional AI co-pilot:** bring your own Anthropic API key for plain-language repair guides and next-step advice.
- **Session history:** audits are saved in your browser's localStorage.

## Quick start
```bash
git clone https://github.com/lord-saviord1/cipher-audit.git
cd cipher-audit
# open index.html in any browser
```

## Use it as an AI agent skill
The same checks are available as a free skill for Claude Code, Codex, Cursor and other SKILL.md agents:

**https://agensi.io/skills/cipher-audit**

It runs locally with the Python standard library, with no API keys and no network calls. Example prompts:
- "Validate the JSON-LD in this page."
- "Analyze my Queries.csv for striking-distance opportunities."

## Privacy
Everything runs in your browser. Data leaves your device only if you use the AI co-pilot, which sends your audit summary to Anthropic with your own key. The key is stored only in your browser's localStorage.

## Scope
A first-pass checker, not a full schema.org or Rich Results validator. For eligibility confirmation, use Google's Rich Results Test.

## Author
Daniel Savior Ozoemena, founder of [Cipher PR](https://cipherpr.me).

## License
MIT

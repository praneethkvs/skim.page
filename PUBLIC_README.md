# skim.page

Get the TL;DR. ASAP.

`skim.page` is a tiny URL shortcut for opening article-summary prompts in the AI assistant you already use.

Add `skim.page/` before any article URL:

```text
skim.page/https://example.com/article
```

skim.page builds a prompt for that article URL and redirects your current tab to your selected AI assistant.

## Why

Sometimes you do not want to read the whole article first. You want a quick summary, a plain-language explanation, a research-style breakdown, or an investor angle.

skim.page gives you a bookmarkable URL pattern for that.

## Examples

Default summary in ChatGPT:

```text
skim.page/https://example.com/article
```

Investor summary in Claude:

```text
skim.page/i/cl/https://example.com/article
```

ELI5 summary in Gemini:

```text
skim.page/e/ge/https://example.com/article
```

## Summary Styles

- `Summary` - quick TL;DR, key takeaways, and why it matters
- `ELI5` - plain language, no jargon
- `Research` - argument, evidence, assumptions, and open questions
- `Investor` - bull case, bear case, market implication, and key risk

## AI Assistants

skim.page currently supports:

- ChatGPT
- Claude
- Gemini
- Perplexity
- Grok

Claude may require an active Claude session before the prompt can open.

## Privacy

skim.page is client-only. It does not scrape articles, run a backend summarizer, create accounts, or store prompts.

The article URL appears in your browser address bar so skim.page can build the prompt. Your browser, hosting infrastructure, and the AI assistant you open may still receive the article URL or generated prompt.

## Limitations

- skim.page does not bypass paywalls.
- skim.page does not summarize articles itself.
- AI assistant URL behavior can change.
- Some assistants may require sign-in.
- URL-only prompts depend on whether the AI assistant can access the article.

## Development

Install dependencies:

```bash
npm install
```

Run locally:

```bash
npm run dev -- --host 127.0.0.1
```

Build:

```bash
npm run build
```

## Tech Stack

- Vite
- React
- TypeScript

## Feedback

Open an issue: https://github.com/praneethkvs/skim.page/issues

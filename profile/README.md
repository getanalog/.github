# Analog lets any AI understand websites as code.

The perception layer for LLMs: webpages in, structured records out.
Deterministic, zero-shot, honest.

```bash
analog get https://quotes.toscrape.com/js/
```

The SDK fetches webpages in a local browser by default, then sends the URL and
rendered page content to Analog for structured extraction. Results return to
the SDK and are saved locally for querying, exporting, and diffing.

**Analog is currently in private alpha.**

## Start here

- [Install Analog](https://getanalog.io/docs/install/)
- [Run the quickstart](https://getanalog.io/docs/quickstart/)
- [Use Analog with Claude, Cursor, and other MCP clients](https://getanalog.io/docs/mcp/)
- [Join the private alpha](https://getanalog.io/signup)

## Public tools

- [`marcato`](https://pypi.org/project/marcato/) — deterministic HTML-to-Markdown conversion on `lxml`.
- [`analog-sdk`](https://pypi.org/project/analog-sdk/) — the `analog` command, Python SDK, and built-in browser.
- [`analog-mcp`](https://pypi.org/project/analog-mcp/) — Analog for MCP-compatible agents.
- [`homebrew-tap`](https://github.com/getanalog/homebrew-tap) — Homebrew distribution for the Analog CLI.

Extraction is zero-shot and uses no LLMs. The default browser visits as an
unauthenticated user; `mode="local"` is the Markdown-only path that sends
nothing. Analog is deliberately blockable automation: it respects `robots.txt`
and does not use stealth, proxies, fingerprint spoofing, or CAPTCHA solving.

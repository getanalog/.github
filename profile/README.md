# Analog lets any AI understand websites as code.

The perception layer for LLMs: webpages in, structured records out.
Deterministic, zero-shot, honest.

The internet was made for human eyes. Analog turns rendered webpages into
structured records that AIs can work with directly: queryable, exportable,
and diffable. Extraction is deterministic and uses no LLMs.

The SDK fetches webpages in a local browser by default, then sends the URL and
rendered page content to Analog for structured extraction. Results return to
the SDK and are saved locally unless disabled.

The default browser visits as an unauthenticated user. Analog respects
`robots.txt` and stays recognizable and blockable: no stealth, proxies,
fingerprint spoofing, or CAPTCHA solving. `mode="local"` is the Markdown-only
path that sends nothing.

## A webpage, as records

```bash
analog get https://books.toscrape.com/
```

Selected fields from one extracted record:

```json
{
  "product": "A Light in the Attic",
  "price": "£51.77",
  "rating": "3/5",
  "badge": "In stock"
}
```

## Start here

**Analog is currently in private alpha.**
[Join the private alpha →](https://getanalog.io/signup)

Already have access?
[Install Analog](https://getanalog.io/docs/install/) ·
[Run the quickstart](https://getanalog.io/docs/quickstart/) ·
[Use Analog through MCP](https://getanalog.io/docs/mcp/)

## Use Analog

- [`analog-sdk`](https://pypi.org/project/analog-sdk/) — the `analog` command,
  Python SDK, and built-in browser.
- [`analog-mcp`](https://pypi.org/project/analog-mcp/) — Analog for
  MCP-compatible agents.
- [`homebrew-tap`](https://github.com/getanalog/homebrew-tap) — Homebrew
  distribution for the Analog CLI.

## From the workshop

- [`marcato`](https://pypi.org/project/marcato/) — deterministic
  HTML-to-Markdown conversion on `lxml`.

## What we value

- **Agentic delight.** We love building things that AIs love: tools that are
  easy to use and honest about their results.
- **Human outcomes.** Behind every AI is a person trying to get something
  done. Getting bad data is worse than getting no data.
- **Safety.** Analog returns deterministic structured data, keeps extraction
  URLs out of its logs, and stays recognizable and blockable on the web.

[Read the note behind Analog →](https://getanalog.io/about/)

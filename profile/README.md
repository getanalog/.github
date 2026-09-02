# Analog lets any AI understand websites as code.

Webpages in, structured records out.

Most ways of giving a webpage to an AI flatten it into a stream of text.
Analog turns the page into the things it contains — products, articles,
events, listings, and other records — so an AI can query, compare, export,
and use them directly. No site-specific schema or API is required.

## Start here

**Analog is currently in private alpha.**
[Join the private alpha →](https://getanalog.io/signup)

Already have access?
[Install Analog](https://getanalog.io/docs/install/) ·
[Run the quickstart](https://getanalog.io/docs/quickstart/) ·
[Use Analog through MCP](https://getanalog.io/docs/mcp/)

## How Analog works

Pages are fetched in a browser on your machine by default. For structured
extraction, the SDK sends the URL and rendered page content to Analog. Results
return to the SDK and are saved locally unless disabled. Authenticated content
is sent only when you explicitly provide it through `html=` or a custom
fetcher. `mode="local"` is the Markdown-only path that sends nothing.

Extraction uses no LLMs. Given the same page URL and HTML, the same engine
produces the same records. A live page's HTML can change between fetches.

## The public toolkit

- [`analog-sdk`](https://pypi.org/project/analog-sdk/) — the `analog` command,
  Python SDK, and built-in browser.
- [`analog-mcp`](https://pypi.org/project/analog-mcp/) — Analog for
  MCP-compatible agents.
- [`marcato`](https://pypi.org/project/marcato/) — deterministic
  HTML-to-Markdown conversion on `lxml`.
- [`homebrew-tap`](https://github.com/getanalog/homebrew-tap) — Homebrew
  distribution for the Analog CLI.

## What we value

- **Agentic delight.** We love building things that AIs love: tools that are
  easy to use and transparent about their capabilities.
- **Human outcomes.** Behind every AI is a person trying to get something
  done. Analog needs to make things easier for people, not just AIs.
- **Safety.** We're building the interface between AI and the internet. AIs
  are obedient, and the internet is not always friendly. So we need to make
  sure that combination stays safe.

[Read more about Analog and its values here →](https://getanalog.io/about/)

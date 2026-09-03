# Analog lets any AI understand websites as code.

Analog is a web interface built for AIs. It converts webpages into the things they contain — products, articles, events, and other records — so AIs can query, compare, export,
and use them directly. No site-specific schema or API is ever required. Just grab Analog and go.

## Start here

**Analog is currently in private alpha.**

Have an invite code?
[Sign up here](https://getanalog.io/signup)

Already signed up?

- [Install Analog](https://getanalog.io/docs/install/)
- [Run the quickstart](https://getanalog.io/docs/quickstart/)
- [Use Analog through MCP](https://getanalog.io/docs/mcp/)

## How Analog works

Analog offers two modes:

1. **Structured extraction (default).**
    - **Render.** Analog renders pages in a browser on your machine.
    - **Send.** The page content is sent to Analog (we never log browsing history).
    - **Map.** Analog converts the page into ordered sections containing labeled records, prose, and navigation. Conversion is deterministic: the same page input always produces the same result.
    - **Use.** We hand the converted result back to you. It's saved locally, where you can query, export, reopen, and compare it using Analog's built-in tools.

2. **Local Markdown conversion (`--mode local`).** This fetches the page and
   converts it to Markdown using `marcato`, our Markdown conversion library.
   Conversion happens entirely on your machine; the page content is never sent
   to Analog. Local mode is free — use it anytime you need to convert
   webpages to Markdown.

## The public toolkit

- [`analog-sdk`](https://pypi.org/project/analog-sdk/) — the `analog` command and Python library.
  - Renders dynamic pages with a built-in headless browser.
  - Maps their records, prose, and navigation in document order.
  - Saves results locally for reopening, querying, exporting, and diffing with the Analog CLI.
  - Includes `marcato` for high-fidelity Markdown conversion.
- [`marcato`](https://pypi.org/project/marcato/) — our free Python library for HTML-to-Markdown conversion, built for accuracy and performance.
  - Preserves document structure, accessible text, and code.
  - Preserves links and image URLs without breaking Markdown syntax.
  - Converts tables when Markdown can represent them faithfully, and preserves
    their content when it cannot.
- [`analog-mcp`](https://pypi.org/project/analog-mcp/) — Analog for
  MCP-compatible agents.
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

# Connect StackTheDeal to your AI

Chatbots are great at conversation and terrible at prices: their built-in
knowledge is months old, so the "deal" they remember is usually dead.
StackTheDeal fixes that. Our deal feed plugs straight into your AI
assistant as a **connector** (it speaks the open MCP standard), so when
you ask for a deal, your assistant checks our live, verified listings —
every price confirmed on the retailer's own page, every deal marked live
or expired — instead of guessing from memory.

**Free. No account. Read-only.** The connector can look at deals; it
can't buy anything, see your data, or change anything.

The same instructions live on the web at
**https://stackthedeal.com/connect-ai/**.

## Connect in under a minute

You only need this one URL:

```
https://stackthedeal.com/mcp
```

### ChatGPT

1. Open **Settings → Connectors** (on Plus/Pro/Team plans, enable
   **Developer mode** under Settings → Connectors → Advanced if you
   don't see the option to add your own).
2. Choose **New connector**.
3. Name: `StackTheDeal Deals` · URL: `https://stackthedeal.com/mcp` ·
   Authentication: **None**.
4. Save, then start a chat and ask for a deal (examples below).

### Claude

1. Open **Settings → Connectors**.
2. Choose **Add custom connector**.
3. Name: `StackTheDeal Deals` · URL: `https://stackthedeal.com/mcp`.
4. Save — no sign-in or API key needed — and ask Claude for a deal.

### Other AI apps

Any app that supports remote MCP servers (streamable HTTP) works the
same way: add a custom/remote server with the URL above. No
authentication. This includes MCP Apps-capable clients (Claude, ChatGPT,
VS Code, Goose), which additionally render deal results as interactive
visual cards.

For clients that take a JSON server configuration, the generic shape is:

```json
{
  "mcpServers": {
    "stackthedeal": {
      "url": "https://stackthedeal.com/mcp"
    }
  }
}
```

## Try asking

- "Find me a coffee maker under $50."
- "What are today's hottest Amazon deals?"
- "Any LEGO sets on sale right now?"
- "Show me tech deals at least 40% off."
- "Cheap flights from New York to Tel Aviv?"
- "Is the air fryer deal from this morning still live?"

Your assistant can browse the newest deals, filter by store, category or
discount, search by keyword, and check whether a specific deal is still
live — and it will link you to the deal's page so you can verify the
price yourself before you buy.

## Why not just ask the AI directly?

| | AI from memory | AI + StackTheDeal connector |
|---|---|---|
| Prices | Months-old training data | Checked on the retailer's page before posting |
| Dead deals | Recommended anyway | Filtered — only live deals are returned |
| Links | Often invented or generic | Real deal pages on stackthedeal.com |
| Coverage | Whatever it memorized | Every live deal we publish, updated with the site |

## The honest fine print

Prices and availability change fast; the retailer's page is always
final. StackTheDeal may earn a commission when you buy through our
links — it never changes your price. The connector is read-only and
collects no personal data; see our
[Privacy Policy](https://stackthedeal.com/privacy-policy/) and
[Disclosure](https://stackthedeal.com/disclosure/) pages.

*Deal data may be shown by your assistant with attribution to
StackTheDeal and a link to the deal's page. No scraping or bulk
redistribution of the full feed without written permission.*

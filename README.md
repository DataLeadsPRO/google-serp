# Google SERP API

> Structured Google search, news, and local results at scale - organic results, news, and local packs as clean JSON.

Part of the **DataLeads** API suite (Search category). Requests render in a real browser with anti-bot handling and protected-page support built in - no proxies to manage, no infrastructure to run.

## Endpoints

| Method | Path | Description |
|---|---|---|
| POST | `/google/search` | V1 Google Search |
| POST | `/google/news` | V1 Google News |
| POST | `/google/local` | V1 Google Local |

## Quick start

```bash
curl -X POST https://data.dataleads.pro/v1/google/search \
  -H 'Content-Type: application/json' \
  -d '{"clientKey": "YOUR_CLIENT_KEY", "query": "best crm for small business"}'
```

Replace `YOUR_CLIENT_KEY` with your key. Get one at [https://data.dataleads.pro](https://data.dataleads.pro) - free tier included.

## MCP server

- **Remote (Streamable HTTP):** `https://data.dataleads.pro/mcp/google-serp`
- **Stdio (Docker):** `docker run -e DATALEADS_API_KEY=yourkey ghcr.io/dataleads/google-serp-mcp:latest`

## Pricing

| Tier | Price | Requests |
|---|---|---|
| Free | $0 | 500/mo |
| Starter | $9/mo | 5,000 |
| Pro | $29/mo | 25,000 |
| Business | $99/mo | 100,000 |
| Enterprise | custom | custom |

Full plan details at [https://data.dataleads.pro](https://data.dataleads.pro).

## License

MIT - see [LICENSE](LICENSE).

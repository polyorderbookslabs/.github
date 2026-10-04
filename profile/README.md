<p align="center">
  <img src="https://raw.githubusercontent.com/polyorderbookslabs/.github/main/profile/logo.svg" width="96" height="96" alt="PolyOrderbooks Labs">
</p>

<h1 align="center">PolyOrderbooks Labs</h1>

<p align="center">
  <strong>Historical Polymarket order book API</strong> — archived L2 bid/ask depth,
  outcome prices, and liquidity metrics for crypto and sports prediction markets.
</p>

<p align="center">
  <a href="https://polyorderbooks.com">Website</a> ·
  <a href="https://api.polyorderbooks.com">API</a> ·
  <a href="https://docs.polyorderbooks.com">Docs</a> ·
  <a href="https://docs.polyorderbooks.com/quickstart">Quickstart</a> ·
  <a href="https://polyorderbooks.com/pricing">Pricing</a>
</p>

---

## What we build

PolyOrderbooks stores **historical** Polymarket market data so you can replay past
order books — not just live snapshots or mid prices.

- **L2 order books** — full bid/ask ladders as `[price, size]` per outcome
- **250ms capture** — every open market, on every plan, including Starter
- **Prices & metrics** — outcome prices, volume, liquidity, spread on the same window
- **Discovery** — search series, events, and markets (crypto and sports)
- **Resolved markets** — settled markets stay queryable, including the winner
- **Read-local API** — your client calls our archive; read paths never hit live Polymarket
- **Backtesting** — fill simulation and slippage against real captured ladders

## Quick example

```bash
export POLYORDERBOOKS_API_KEY="pob_your_key_here"

curl -s -H "X-API-Key: $POLYORDERBOOKS_API_KEY" \
  "https://api.polyorderbooks.com/v1/markets?search=bitcoin&limit=5"
```

Create a free API key: [polyorderbooks.com/signup](https://polyorderbooks.com/signup)

## Open source

| Repository | What it is |
| --- | --- |
| [polyorderbooks-python](https://github.com/polyorderbookslabs/polyorderbooks-python) | Official Python client — [`pip install polyorderbooks`](https://pypi.org/project/polyorderbooks/) |
| [mcp-server](https://github.com/polyorderbookslabs/mcp-server) | MCP server for Claude, Cursor, and other MCP clients |
| [python-examples](https://github.com/polyorderbookslabs/python-examples) | Runnable examples for the Python SDK |
| [n8n-templates](https://github.com/polyorderbookslabs/n8n-templates) | n8n workflows for historical order book data |
| [polymarket-orderbook-research](https://github.com/polyorderbookslabs/polymarket-orderbook-research) | Reproducible measurement scripts behind the published research |

## Contact

- Email: [contact@polyorderbooks.com](mailto:contact@polyorderbooks.com)
- X: [@polyorderbooks](https://x.com/polyorderbooks)

---

Independent data product. Not affiliated with or endorsed by Polymarket.
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

<p align="center">
  <a href="https://pypi.org/project/polyorderbooks/"><img src="https://img.shields.io/pypi/v/polyorderbooks?label=polyorderbooks&color=3775a9" alt="PyPI — polyorderbooks"></a>
  <a href="https://pypi.org/project/polyorderbooks-backtest/"><img src="https://img.shields.io/pypi/v/polyorderbooks-backtest?label=polyorderbooks-backtest&color=3775a9" alt="PyPI — polyorderbooks-backtest"></a>
  <a href="https://www.npmjs.com/package/@polyorderbooks/mcp-server"><img src="https://img.shields.io/npm/v/@polyorderbooks/mcp-server?label=mcp-server&color=cb3837" alt="npm — @polyorderbooks/mcp-server"></a>
  <a href="https://doi.org/10.5281/zenodo.22084114"><img src="https://img.shields.io/badge/DOI-10.5281%2Fzenodo.22084114-1682d4" alt="DOI 10.5281/zenodo.22084114"></a>
  <a href="https://github.com/polyorderbookslabs/polyorderbooks-python/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-3da639" alt="License: MIT"></a>
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

Verifiable and citable: **1B+ L2 snapshots** across **800k+ markets**, published as a
CC BY 4.0 dataset with a [Zenodo DOI (10.5281/zenodo.22084114)](https://doi.org/10.5281/zenodo.22084114).

## Quick example

```bash
export POLYORDERBOOKS_API_KEY="pob_your_key_here"

curl -s -H "X-API-Key: $POLYORDERBOOKS_API_KEY" \
  "https://api.polyorderbooks.com/v1/markets?search=bitcoin&limit=5"
```

Create a free API key: [polyorderbooks.com/signup](https://polyorderbooks.com/signup)

## Open source

### Start here

| Repository | What it is |
| --- | --- |
| [polyorderbooks-python](https://github.com/polyorderbookslabs/polyorderbooks-python) | Official Python client — [`pip install polyorderbooks`](https://pypi.org/project/polyorderbooks/) |
| [polyorderbooks-backtest-python](https://github.com/polyorderbookslabs/polyorderbooks-backtest-python) | Replay-accurate backtesting library — [`pip install polyorderbooks-backtest`](https://pypi.org/project/polyorderbooks-backtest/) |
| [backtest-strategies](https://github.com/polyorderbookslabs/backtest-strategies) | Runnable strategy cookbook for backtesting against real L2 order books |
| [mcp-server](https://github.com/polyorderbookslabs/mcp-server) | MCP server for Claude, Cursor, and other MCP clients — [`@polyorderbooks/mcp-server`](https://www.npmjs.com/package/@polyorderbooks/mcp-server) |

### More

| Repository | What it is |
| --- | --- |
| [python-examples](https://github.com/polyorderbookslabs/python-examples) | Runnable examples for the Python SDK |
| [n8n-templates](https://github.com/polyorderbookslabs/n8n-templates) | n8n workflows for historical order book data |
| [polymarket-orderbook-research](https://github.com/polyorderbookslabs/polymarket-orderbook-research) | Reproducible measurement scripts behind the published research |

## Contact

- Email: [contact@polyorderbooks.com](mailto:contact@polyorderbooks.com)
- X: [@polyorderbooks](https://x.com/polyorderbooks)

---

Independent data product. Not affiliated with or endorsed by Polymarket.

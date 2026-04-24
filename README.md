# boatpartsmanual-mcp

**Canonical product identity for marine parts — resolve SKUs, OEM numbers, and part numbers across manufacturers, vendors, and retailers to one canonical product.**

`boatpartsmanual-mcp` is a read-only [Model Context Protocol](https://modelcontextprotocol.io/) server for the marine parts catalog at [BoatPartsManual.com](https://boatpartsmanual.com/). It canonicalises product identity across **manufacturers, vendors, and retailers** — given a SKU, OEM number, or manufacturer part number from any source, the server resolves to a canonical product and exposes the equivalent identifiers at other manufacturers, wholesalers, and online retailers.

Basic tools are **free at launch**. Catalog coverage expands weekly.

> **Status:** pre-launch stub, version `0.0.1`. The real MCP server ships in the next few days. This package reserves the name and lets you `pip install` / `npm install` the future runtime from the same identifier.

---

## Why this exists

The marine parts ecosystem is fragmented: the same physical part shows up under a dozen different SKUs across OEMs, wholesalers, and online retailers. BoatPartsManual.com has been mapping those identifiers to a single canonical product for the public catalog. This MCP server exposes that same identity graph to AI agents — resolve any source's SKU to the canonical part, then list all the equivalent SKUs other sources carry.

## Install

```bash
pip install boatpartsmanual-mcp
```

```bash
npm install boatpartsmanual-mcp
```

## Basic tools at launch (free tier)

- **Product identity** — resolve an SKU, OEM number, GTIN, or manufacturer label to a canonical product (identity, taxonomy path, primary image) and the equivalent identifiers at other manufacturers, vendors, and retailers. Anchored queries only; no catalog enumeration.
- **Category tree** — walk the public category hierarchy from a known parent anchor.
- **Brand directory** — look up manufacturers and brands in the catalog.

Compatibility graphs, equivalence edges, and evidence-heavy flows are planned as **separate, paid surfaces** — they are not part of the free basic tier.

## Documentation

Full docs, registration for API keys (when required), and launch announcements:

- https://boatpartsmanual.com/docs/mcp

## Licence

Client packages (this repository, the PyPI package, the npm package) are licensed under **Apache License 2.0** — see [`LICENSE`](./LICENSE) and [`NOTICE`](./NOTICE).

The hosted MCP endpoint at `mcp.boatpartsmanual.com` is operated by Oish AB and is subject to the [BoatPartsManual.com terms of service](https://boatpartsmanual.com/terms). An MCP-specific terms section will be added when the server goes live. Commercial and usage terms for paid tiers (if any) will be announced on a dedicated pricing page — basic tools are free at launch.

## Attribution

Responses from the hosted server carry attributed outbound purchase links where applicable, so the catalog remains sustainable.

## Contact

- General: [info@boatpartsmanual.com](mailto:info@boatpartsmanual.com)
- MCP early notifications: [info@boatpartsmanual.com](mailto:info@boatpartsmanual.com?subject=MCP%20early%20access) (subject: `MCP early access`)

## About Oish AB

`boatpartsmanual-mcp` is developed and operated by **Oish AB**, a Swedish limited company. BoatPartsManual.com is an Oish AB product.

"BoatPartsManual" is an unregistered trademark of Oish AB.

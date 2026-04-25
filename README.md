# boatpartsmanual-mcp

Read-only Model Context Protocol endpoint for the marine parts catalog at
[BoatPartsManual.com](https://boatpartsmanual.com/).

The hosted endpoint is:

```text
https://mcp.boatpartsmanual.com/mcp
```

Use an MCP client that supports Streamable HTTP. The npm and PyPI packages are
small metadata/launcher packages that print the live endpoint and documentation
URL.

## Install

```bash
pip install boatpartsmanual-mcp
```

```bash
npm install boatpartsmanual-mcp
```

## Available tools

- **Product lookup** - resolve a name, SKU, OEM number, GTIN, or manufacturer
  label to matching BoatPartsManual.com catalog products. Responses include
  catalog facts, taxonomy path, attribution, and BoatPartsManual.com product
  links.
- **Brand directory** - look up manufacturers and brands in the catalog.

Anchored questions are supported. Bulk catalog enumeration is not supported.

## Documentation

https://boatpartsmanual.com/docs/mcp

## Licence

Client packages are licensed under Apache License 2.0. See `LICENSE` and
`NOTICE`.

The hosted MCP endpoint is operated by Oish AB and is subject to the
[BoatPartsManual.com terms of service](https://boatpartsmanual.com/terms).

## Contact

- General: [info@boatpartsmanual.com](mailto:info@boatpartsmanual.com)

## About Oish AB

`boatpartsmanual-mcp` is developed and operated by Oish AB, a Swedish limited
company. BoatPartsManual.com is an Oish AB product.

"BoatPartsManual" is an unregistered trademark of Oish AB.

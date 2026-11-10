# Nigeria Import Export Data MCP

**Nigeria Customs Data: Importers, Suppliers & HS Codes.** Nigeria import export data for your AI assistant. Search Nigeria customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Nigeria trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/nigeria
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Nigeria: the server tells your AI to filter on `NG` unless you ask about another country

## Nigeria data coverage

- **Years:** 2019–2025
- **Records:** Import declarations: Nigerian importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `NG` (use `buyerCountry: "NG"` for imports into Nigeria)
- **Common products:** wheat (HS 1001), sugar (HS 1701), refined fuel (HS 2710), cars (HS 8703)

> Banks often appear as the declared party on letters of credit.

## Notable traders in the data

Companies that appear most often in recent Nigeria records (by number of declaration lines, not value):

**Importers**

- Flour Mills of Nigeria
- Dangote Sugar Refinery
- Vitol
- Shell Western Supply and Trading

## Example prompts

- *"Who are the top importers of wheat (HS 1001) into Nigeria?"*
- *"What does Dangote Sugar Refinery import, and from where?"*
- *"List Nigerian importers of refined fuel (HS 2710) in 2024"*
- *"Which suppliers ship to Flour Mills of Nigeria?"*
- *"Show recent import shipments of cars (HS 8703) into Nigeria"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Nigeria import data, Nigeria export data, Nigeria customs data, Nigeria shipment data, importers in Nigeria, Nigeria buyers and suppliers, HS code search, Nigeria customs data, Nigeria Customs Service import data, importers in Nigeria, Form M

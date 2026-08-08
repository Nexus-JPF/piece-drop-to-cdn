# piece-drop-to-cdn

[Activepieces](https://www.activepieces.com/) piece for [Drop to CDN](https://droptocdn.com) — upload files and get instant public CDN URLs.

## Install

In Activepieces: **Settings → My Pieces → Install Piece** → enter:

```
piece-drop-to-cdn
```

Works on Activepieces Cloud and self-hosted instances that allow custom pieces.

## Connect

1. Create an API key at [Drop to CDN → Settings → API keys](https://droptocdn.com/dashboard/settings) (`dtc_...`).
2. In Activepieces: **Connections → Drop to CDN** → paste your API key.

## Actions

| Action | Description |
|--------|-------------|
| **Upload File** | Upload a file (or URL) → public CDN URL |
| **Get File Information** | CDN URL and metadata by file ID |
| **Delete File** | Permanently delete by ID |

Auth: `Authorization: Bearer dtc_...` (validated via `GET /v1/profile`).

## HTTP Request fallback

If you cannot install the piece, use Activepieces **HTTP** steps against `https://api.droptocdn.com/v1`. See [droptocdn.com/integrations/activepieces](https://droptocdn.com/integrations/activepieces).

## Development

```bash
npm install
npm run build
npm test
```

## Source

Developed by [Drop to CDN](https://droptocdn.com). This public repo is synced from the private monorepo for npm publishing.

## License

MIT

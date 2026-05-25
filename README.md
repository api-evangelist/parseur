# Parseur

AI-powered document and email parsing platform that automatically extracts structured data from PDFs, emails, scans, and arbitrary file uploads, then routes JSON / CSV / Excel records into downstream systems via webhooks, native integrations, or its REST API. Headquartered in Singapore, Parseur combines Vision AI, Text AI, template-based extraction, OCR, normalization, and field validation behind a per-mailbox forwarding email address, and connects to 1,000+ applications including Zapier, Make, n8n, Power Automate, Google Sheets, Airtable, Salesforce, Excel, and Slack.

- Website: https://parseur.com
- App / Portal: https://app.parseur.com
- Developer Documentation: https://developer.parseur.com/
- Support Center: https://help.parseur.com/
- OpenAPI Specification: https://api.parseur.com/openapi.json
- API Keys: https://app.parseur.com/account/api-keys
- Pricing: https://parseur.com/pricing
- Status: https://status.parseur.com
- GitHub: https://github.com/parseur

## API

| Property | Value |
|---|---|
| Name | Parseur API |
| Base URL | `https://api.parseur.com` |
| OpenAPI | [`openapi/parseur-openapi.yml`](openapi/parseur-openapi.yml) (source: https://api.parseur.com/openapi.json) |
| Spec version | OpenAPI 3.1.0 |
| Authentication | `Authorization: Token <API_KEY>` header |
| Rate Limits | 5 req/sec per IP, burst 20 (HTTP 429 on excess) |
| Operations | 29 across mailboxes (parsers), documents, templates, webhooks, exports, bootstrap |

### Operation Surface

**Documents**

- `GET /parser/{id}/document_set` — List documents in a mailbox
- `GET /document/{id}` — Get a document
- `DELETE /document/{id}` — Delete a document
- `GET /document/{id}/log_set` — Get document logs
- `POST /parser/{id}/upload` — Upload a binary document
- `POST /email` — Upload an email/text document
- `POST /document/{id}/process` — Reprocess a document
- `POST /document/{id}/skip` — Skip a document
- `POST /document/{id}/copy/{target_mailbox_id}` — Copy a document

**Mailboxes (Parsers)**

- `GET /parser` — List mailboxes
- `POST /parser` — Create a mailbox
- `GET /parser/{id}` — Get a mailbox
- `PUT /parser/{id}` — Update a mailbox
- `DELETE /parser/{id}` — Delete a mailbox
- `GET /parser/{id}/schema` — Get mailbox schema
- `POST /parser/{id}/copy` — Copy a mailbox

**Templates**

- `GET /parser/{id}/template_set` — List templates in a mailbox
- `GET /template/{id}` — Get a template
- `DELETE /template/{id}` — Delete a template
- `POST /template/{id}/copy/{target_mailbox_id}` — Copy a template

**Custom Downloads (Export Configs)**

- `GET /parser/{id}/export_config` — List custom downloads
- `POST /parser/{id}/export_config` — Create a custom download
- `PATCH /parser/{mailbox_id}/export_config/{id}` — Update a custom download
- `DELETE /parser/{mailbox_id}/export_config/{id}` — Delete a custom download

**Webhooks**

- `POST /webhook` — Create a webhook
- `POST /parser/{mailbox_id}/webhook_set/{id}` — Enable a webhook
- `DELETE /parser/{mailbox_id}/webhook_set/{id}` — Disable a webhook
- `DELETE /webhook/{id}` — Delete a webhook

**Bootstrap**

- `GET /bootstrap` — Get bootstrap config

## SDKs and Tooling

- [parseur-py](https://github.com/parseur/parseur-py) — Official Python client (MIT).
- [parseur-n8n-node](https://github.com/parseur/parseur-n8n-node) — Official n8n community node (MIT, TypeScript).

## Pricing

Volume-based on pages processed (1 credit = 1 page).

| Plan | Pages / month | Price | Notes |
|---|---|---|---|
| Free | 20 | $0 | Forever free, credits valid 1 year, 90-day retention |
| Base | up to 3,000 | Variable | 1-year retention, chat + email support |
| Scale | up to 1,000,000 | Variable | Lowest cost per page, advanced post-processing, up to 100 users, unlimited retention |
| Enterprise | up to 10,000,000 | Custom | Unlimited users, POs, custom terms, security questionnaire |

## Repository Layout

```
parseur/
├── apis.yml                              # API Commons profile (APIs.json 0.20)
├── README.md                             # This file
└── openapi/
    └── parseur-openapi.yml               # Parseur OpenAPI 3.1 (mirrored from api.parseur.com)
```

## Maintainer

Kin Lane — kin@apievangelist.com — API Evangelist Network

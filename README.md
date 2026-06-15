# Parseur (parseur)

Parseur is an AI-powered document and email parsing platform headquartered in Singapore that automatically extracts structured data from PDFs, emails, scanned documents, and arbitrary file uploads, then routes the resulting JSON, CSV, or Excel records into downstream systems via webhooks, native integrations, or its REST API. The platform combines Vision AI, Text AI, template-based extraction, OCR, normalization, and field validation behind a forwarding email address per mailbox, and connects to more than 1,000 applications including Zapier, Make, n8n, Power Automate, Google Sheets, Airtable, Salesforce, Excel, and Slack. Parseur exposes a public REST API at https://api.parseur.com with an OpenAPI 3.1 specification covering mailbox (parser) management, document upload and lifecycle, templates, custom export configurations, and webhook subscriptions, secured with a per-account Token-based Authorization header. Pricing is volume-based on pages processed, with a permanent free tier (20 pages/month) and Base, Scale, and Enterprise tiers that scale up to 10 million pages per month.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/parseur/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/parseur/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- Document Parsing
- Document Processing
- Document Extraction
- Email Parsing
- OCR
- Data Extraction
- Vision AI
- Automation
- Webhooks
- Mailboxes
- SaaS

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Parseur API

The Parseur REST API exposes 29 operations across mailboxes (parsers), documents, templates, custom downloads (export configs), webhooks, and account bootstrap. Documents can be ingested as binary uploads to /parser/{id}/upload or as email/text payloads to /email; parsing is asynchronous, with results retrievable via /document/{id} once status transitions to processed. Webhooks deliver real-time events to your endpoint and can be enabled/disabled per mailbox. Authentication uses a Token-prefixed Authorization header carrying the account API key from the Parseur Account Overview. Base URL is https://api.parseur.com and rate limits are 5 requests/second per IP with a burst of 20.

- **Human URL:** [https://developer.parseur.com/](https://developer.parseur.com/)
- **Base URL:** `https://api.parseur.com`

#### Tags

- Documents
- Mailboxes
- Templates
- Webhooks
- Exports
- AI
- OCR

#### Properties

- [Documentation](https://developer.parseur.com/)
- [Documentation](https://help.parseur.com/en/articles/3566128-use-parseur-document-parsing-api)
- [Documentation](https://help.parseur.com/en/articles/3566112-send-documents-to-parseur-using-the-api)
- [OpenAPI](openapi/parseur-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/parseur.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/parseur.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [SDK](https://github.com/parseur/parseur-py)
- [Authentication](https://developer.parseur.com/)
- [Rate Limits](https://developer.parseur.com/)
- [Webhooks](https://developer.parseur.com/)

## Common Properties

- [Website](https://parseur.com)
- [Portal](https://app.parseur.com)
- [Sign Up](https://app.parseur.com/accounts/signup/)
- [Login](https://app.parseur.com/accounts/login/)
- [Documentation](https://developer.parseur.com/)
- [Support Center](https://help.parseur.com/)
- [OpenAPI](https://api.parseur.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [A P I Keys](https://app.parseur.com/account/api-keys)
- [About](https://parseur.com/about)
- [Blog](https://parseur.com/blog/)
- [Pricing](https://parseur.com/pricing)
- [Integrations](https://parseur.com/integrations)
- [Contact](https://parseur.com/contact)
- [Careers](https://parseur.com/jobs)
- [Terms of Service](https://parseur.com/terms)
- [Privacy Policy](https://parseur.com/privacy)
- [Security](https://help.parseur.com/en/articles/4578268-security-and-privacy-at-parseur)
- [Status Page](https://status.parseur.com)
- [Git Hub](https://github.com/parseur)
- [Twitter](https://twitter.com/parseur)
- [LinkedIn](https://www.linkedin.com/company/parseur.com)
- [YouTube](https://www.youtube.com/@parseur)
- [Reddit](https://www.reddit.com/r/Parseur/)
- [Plans](https://parseur.com/pricing)
- [Rate Limits](https://developer.parseur.com/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

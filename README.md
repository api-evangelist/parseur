# Parseur (parseur)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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

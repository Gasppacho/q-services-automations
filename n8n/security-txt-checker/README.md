# Security\.txt Checker — Security Contact Finder — n8n automation

This n8n automation use case runs [Security\.txt Checker — Security Contact Finder](https://apify.com/q_services/security-txt-checker), polls the exact Apify run, and fails explicitly when the run is not successful.

Trigger one bounded portfolio run, poll the same Actor run to completion, retrieve structured domain statuses, compare them with the previous successful cycle, and route only new missing or expired exceptions through an explicit success or failure path\.

**Audience:** Managed security providers and vendor\-risk teams responsible for recurring checks across customer and supplier domain portfolios


## Install

1. Import `workflow.json` into n8n.
2. Expose `APIFY_TOKEN` to n8n as an environment variable or replace the expressions with an n8n credential.
3. Review the public input in the **Prepare safe input** node.
4. Connect **Get dataset items** to Slack, email, Google Sheets, or a webhook.
5. Activate the workflow only after a successful manual execution.

No credential or personal data is included in this repository.

## Tested input

```json
{
  "includeRootFallback": false,
  "maxResults": 1,
  "proxyConfiguration": {
    "useApifyProxy": true
  },
  "startUrls": [
    "https://securitytxt.org"
  ]
}
```

## Links

- [Technical guide](https://q-services.fr/blog/security-txt-checker-2026-07-27-growth-guide/)
- [Apify Store](https://apify.com/q_services/security-txt-checker)

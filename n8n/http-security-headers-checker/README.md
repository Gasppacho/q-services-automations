# HTTP Security Headers Checker — n8n automation

This n8n automation use case runs [HTTP Security Headers Checker](https://apify.com/q_services/http-security-headers-checker), polls the exact Apify run, and fails explicitly when the run is not successful.

Déclenche un audit borné, suit le même run Apify jusqu’à son état terminal, récupère le dataset et transmet les écarts à une destination d’équipe avec une branche d’échec explicite\.

**Audience:** Responsables sécurité, agences web et équipes plateforme qui gèrent plusieurs domaines publics


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
  "startUrls": [
    "https://example.com"
  ],
  "maxResults": 1,
  "proxyConfiguration": {
    "useApifyProxy": false
  }
}
```

## Links

- [Technical guide](https://q-services.fr/blog/http-security-headers-checker-2026-07-24-growth-guide/)
- [Apify Store](https://apify.com/q_services/http-security-headers-checker)

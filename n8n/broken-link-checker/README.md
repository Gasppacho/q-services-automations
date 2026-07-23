# Broken Link Checker — Find All 404s &amp; Dead Links on Any Website — n8n automation

This n8n automation use case runs [Broken Link Checker — Find All 404s &amp; Dead Links on Any Website](https://apify.com/q_services/broken-link-checker), polls the exact Apify run, and fails explicitly when the run is not successful.

Planifie un contrôle borné, démarre le Broken Link Checker via l&\#x27;API Apify, suit le même run jusqu&\#x27;à son état terminal, récupère le dataset et transmet les incidents à une destination configurable avec une branche d&\#x27;échec explicite\.

**Audience:** Agences SEO, équipes web et responsables e\-commerce qui maintiennent plusieurs sites et doivent détecter les régressions de liens dans la durée


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
    "https://the-internet.herokuapp.com/status_codes"
  ],
  "maxPages": 1,
  "checkExternalLinks": false
}
```

## Links

- [Technical guide](https://q-services.fr/blog/broken-link-checker-2026-07-23-growth-guide/)
- [Apify Store](https://apify.com/q_services/broken-link-checker)

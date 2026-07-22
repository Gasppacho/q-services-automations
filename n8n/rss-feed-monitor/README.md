# RSS Feed Monitor — n8n automation

This workflow runs [RSS Feed Monitor](https://apify.com/q_services/rss-feed-monitor) every 24 hours, polls the Apify run, retrieves its dataset, and fails explicitly when the run is not successful.

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
  "keywords": [],
  "maxResults": 10,
  "proxyConfiguration": {
    "useApifyProxy": false
  },
  "startUrls": [
    "https://q-services.fr/blog/rss.xml"
  ]
}
```

## Links

- [Technical guide](https://q-services.fr/blog/automate-rss-feed-monitor-with-apify/)
- [Apify Store](https://apify.com/q_services/rss-feed-monitor)

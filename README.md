# Q Services Automations

Public, runnable automation examples for the [Q Services Apify Actor catalog](https://apify.com/q_services).

## Structure

- `n8n/` — scheduled scraping, monitoring, enrichment, and data workflows
- `github-actions/` — CI, DevSecOps, Terraform, and dependency checks
- `mcp/` — executable MCP and agent guardrail scenarios
- `api-examples/` — minimal Apify API examples
- `catalog.json` — machine-readable automation catalog

Every example is standalone, contains no credentials or personal data, links to its canonical Q Services technical guide and Apify Store page, and documents a tested input. Credentials are represented only by environment-variable placeholders.

## Security

Never commit tokens. Review imported workflows before activation and use the credential store provided by the automation platform.

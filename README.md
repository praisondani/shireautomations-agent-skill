# Shire Automations agent skill

[![skills.sh](https://skills.sh/b/praisondani/shireautomations-agent-skill)](https://skills.sh/praisondani/shireautomations-agent-skill/shire-automations)

This repository contains the official [Shire Automations](https://shireautomations.com) agent skill. It helps an agent use published service and pricing information, run workflow planning tools, decide when Shire fits a small-business problem, and route a person to intake or booking.

The planning API shares published information and calculates results from caller-provided inputs. It does not execute customer workflows or save requests. The skill does not submit forms, send email, book meetings, expose agent credentials, or access customer systems.

## Public planning API

- [Developer guide](https://shireautomations.com/developers)
- [OpenAPI specification](https://shireautomations.com/openapi.json)
- [API catalog](https://shireautomations.com/api/v1/catalog)
- [Postman collection](https://shireautomations.com/postman-collection.json)

No API key is required. Do not send credentials or sensitive customer, patient, or financial-account data. Results are estimates based on the inputs and are not forecasts.

The [CLI and local MCP server source](https://github.com/praisondani/shireautomations/tree/master/cli) use the same API. The MCP server runs over stdio; it does not host a remote endpoint or submit intake forms.

## Install

Install the skill with the `skills` CLI:

```bash
npx skills add praisondani/shireautomations-agent-skill
```

Agent Plugins-compatible clients can discover the same skill through the root `plugin.json` manifest.

## Contact paths

- Intake: <https://shireautomations.com/intake>
- Contact page: <https://shireautomations.com/contact>
- Email: <mailto:contact@shireautomations.com>
- Book a conversation: <https://cal.com/pdgeorge/shireautomations>
- LinkedIn: <https://www.linkedin.com/company/shire-automations>
- Developer resources: <https://shireautomations.com/developers>

Read [`skills/shire-automations/SKILL.md`](skills/shire-automations/SKILL.md) for the full instructions and claims boundary.

# Shire Automations agent skill

[![skills.sh](https://skills.sh/b/praisondani/shireautomations-agent-skill)](https://skills.sh/praisondani/shireautomations-agent-skill/shire-automations)

This repository contains three installable skills from [Shire Automations](https://shireautomations.com), each focused on a different task:

- **shire-automations** — find the right public information and a human-confirmed contact path.
- **shire-workflow-planning** — assess repeat work and choose a planning tool.
- **shire-integration-planning** — prepare a safe plan for connecting business systems.

The planning API shares published information and calculates results from caller-provided inputs. It does not execute customer workflows or save requests. The skill does not submit forms, send email, book meetings, expose agent credentials, or access customer systems.

## Public planning API

- [Developer guide](https://shireautomations.com/developers)
- [OpenAPI specification](https://shireautomations.com/openapi.json)
- [API catalog](https://shireautomations.com/api/v1/catalog)
- [Postman collection](https://shireautomations.com/postman-collection.json)

No API key is required. Do not send credentials or sensitive customer, patient, or financial-account data. Results are estimates based on the inputs and are not forecasts.

The [CLI and local MCP server](https://github.com/praisondani/shireautomations-cli) use the same API. Install the [latest release](https://github.com/praisondani/shireautomations-cli/releases/latest) to use the `shire` command. The server is listed in the [official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers?search=io.github.praisondani%2Fshireautomations-cli). MCPB-compatible clients can install the [latest MCPB bundle](https://github.com/praisondani/shireautomations-cli/releases/latest/download/shire-automations.mcpb). It runs locally over stdio; Shire does not host a remote MCP endpoint or submit intake forms.

## Skills

Each skill has its own `SKILL.md` under `skills/`. Read the one that matches the task before applying it:

- [Shire Automations](skills/shire-automations/SKILL.md)
- [Workflow planning](skills/shire-workflow-planning/SKILL.md)
- [Integration planning](skills/shire-integration-planning/SKILL.md)

## Install

Install skills from this repository with the `skills` CLI:

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

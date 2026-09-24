# Shire Automations agent skill

[![skills.sh](https://skills.sh/b/praisondani/shireautomations-agent-skill)](https://skills.sh/praisondani/shireautomations-agent-skill)

This repository contains the official [Shire Automations](https://shireautomations.com) agent skill. It helps an agent decide when Shire Automations fits a small-business workflow problem and route the person to published pricing, intake, email, or booking.

The skill is intentionally a contact and discovery guide. It does not submit forms, send email, book meetings, expose a public automation API, or provide agent credentials.

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

Read [`skills/shire-automations/SKILL.md`](skills/shire-automations/SKILL.md) for the full instructions and claims boundary.

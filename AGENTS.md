# Shire Automations agent skill repository

This public repository packages the official Shire Automations agent skill. Read `skills/shire-automations/SKILL.md` before changing the skill or its public contact paths.

## Scope

- Keep the skill focused on choosing a published Shire Automations service and helping a person start a conversation.
- Use only public URLs from `shireautomations.com`, the published booking page, the public LinkedIn page, and this repository.
- Keep the portable Agent Plugin manifest at `plugin.json` and the skill at `skills/shire-automations/SKILL.md`.

## Safety and claims

- Do not add a public API, OAuth flow, MCP server, or other capability that Shire Automations does not operate.
- Do not submit an intake form, send email, or book a meeting for a person without an explicit confirmation step.
- Do not add testimonials, revenue claims, guaranteed ROI, or unverified time-savings claims.
- Keep pricing aligned with `https://shireautomations.com/pricing.md`.

## Local checks

Run these checks before publishing changes:

```bash
jq empty plugin.json
test -s skills/shire-automations/SKILL.md
rg -n "shireautomations.com|contact@shireautomations.com|cal.com" skills/shire-automations/SKILL.md
```

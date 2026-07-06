# Public Redaction Rules

Use this checklist before publishing any portfolio page, screenshot, README, demo, or case study.

## Never Publish

- `.env` files or environment variable values
- Slack tokens, OpenAI keys, GitHub tokens, Railway tokens, SCIM tokens, app-level tokens
- Slack workspace, org, team, channel, user, trigger, list, canvas, or app IDs
- raw seed data that enables someone to recreate the full demo system
- full prompts or instruction files that encode reusable delivery strategy
- private customer names, internal team names, private channel names, or employee names
- live deployment admin URLs, dashboards, or CLI output containing account identifiers

## Publish Only After Sanitizing

- screenshots: crop or blur workspace names, people names, message text, URLs, IDs, and admin panels
- architecture diagrams: show component types, not exact infrastructure names
- case studies: describe the problem and engineering approach, not the full recipe
- metrics: use rounded or approximate numbers unless the number is already public-safe
- code snippets: keep small and generic; avoid handlers that reveal token scopes, channel routing, or private schemas

## Safe Language

Prefer:

- "multi-workspace Slack environment"
- "enterprise collaboration platform"
- "internal workflow app"
- "synthetic financial services demo"
- "risk graph and evidence retrieval"
- "server-rendered internal portal"

Avoid:

- exact customer-like demo names unless explicitly approved
- specific Slack plan or product-tier names (for example, do not write "Enterprise Grid"); use neutral phrasing such as "multi-workspace Slack environment" or "enterprise collaboration platform" when the exact tier is not certain
- other product-plan labels that may be inaccurate or distracting
- "we can replicate this exact operating model" claims
- secret operational details such as provisioning steps, auth/identity workarounds, or seed generation tricks

## Screenshot Standard

Each public screenshot should pass this quick scan:

- No visible token, ID, private email, internal URL, or admin-only page
- No private person or company name unless intentionally fictional and approved
- No detailed channel list that reveals a copyable demo taxonomy
- No direct code or prompt that gives away the full build recipe
- The screenshot still proves the skill: UX, workflow, dashboard, deployment, or integration

## Recruiter-Friendly Proof

A public artifact is strong enough when it shows:

- the problem
- the role
- the architecture at a high level
- the delivered user experience
- the deployment or verification result
- what was learned

It does not need to reveal the private implementation map.


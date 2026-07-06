# Engineering Work Portfolio

This repository is a public-safe career portfolio hub. It summarizes selected engineering work across Slack apps, internal workflow systems, RAG/MCP prototypes, data safety automation, and enterprise demo portals without exposing customer data, private prompts, tokens, Slack workspace identifiers, or copyable internal playbooks.

## Positioning

I build practical internal productivity systems that combine:

- Slack app workflows and App Home UX
- Approval, request, and case management flows
- RAG and MCP-style knowledge retrieval
- Data safety and file scanning automation
- Enterprise portal prototypes and demo environments
- Railway/Docker deployment and operational handoff docs

The emphasis is not only on code, but on full delivery: product framing, data modeling, UX, automation, deployment, verification, and documentation.

Recent work includes a large synthetic financial-services collaboration environment spanning a dozen-plus workspaces and hundreds of directory profiles, together with the workflow app, internal portal, and retrieval layer built on top of it. Each piece was designed, built, deployed to a realistic runtime, and documented for handoff.

## Selected Work Areas

| Area | Public-safe summary | Evidence of execution |
|---|---|---|
| Slack workflow systems | Built request, approval, routing, notification, and App Home flows for operational teams. | Modal flows, approval state handling, DM notifications, Slack List/Canvas patterns, deployment guides. |
| Risk and knowledge retrieval | Built graph/RAG-style tools that connect systems, vendors, incidents, documents, and regulations into queryable paths. | MCP tool surface, SQLite/PostgreSQL-backed graph data, smoke tests, demo query sets. |
| Internal portals | Built server-rendered internal portal prototypes that reuse Slack/demo data for directory, approvals, documents, vendors, and risk dashboards. | FastAPI/Jinja2, bundled data snapshot, Dockerfile, Railway deployment. |
| File safety automation | Built Slack-based file scanning and gateway patterns for sensitive document workflows. | File download/parsing, OCR-ready pipeline, policy scoring, admin review path. |
| News and briefing automation | Built scheduled collection and categorization apps for business intelligence and team briefings. | RSS/API ingestion, deduplication, category routing, scheduled Slack posting. |
| Reusable delivery system | Consolidated app-building instructions, skills, checklists, and review playbooks for faster repeat delivery. | Studio-style instruction set, deployment checklists, reusable QA patterns. |

## Case Studies

- [Case Study 01: Enterprise Slack Operating System](docs/case-study-enterprise-slack-os.md)
- [Case Study 02: Risk Graph and RAG Workbench](docs/case-study-risk-graph-rag.md)
- [Case Study 03: Internal Portal and Workflow Hub](docs/case-study-portal-workflow.md)
- [Case Study 04: File Safety and Compliance Automation](docs/case-study-file-safety.md)

## Public Redaction Rules

This hub intentionally avoids:

- API keys, tokens, secrets, credentials, or environment files
- Slack team, channel, user, app, trigger, list, or canvas IDs
- customer-specific names unless already public and intentionally sanitized
- full internal prompts, seed data, instruction files, or exact operating procedures
- raw screenshots containing real workspace names, people, messages, URLs, or identifiers

See [Public Redaction Rules](docs/redaction-rules.md) for the working standard.

## How to Review This Portfolio

For recruiters and hiring teams, the best signal is the repeated pattern across projects:

1. Translate an operational problem into a usable internal app.
2. Model the domain with realistic data and workflow states.
3. Build Slack-native or portal-native interfaces.
4. Deploy and verify the app in a realistic environment.
5. Document the system so another operator can run it.

## Status

Draft portfolio hub. Content is intentionally high-level and public-safe. Private repositories and sensitive implementation details can be discussed selectively during interviews.

## Contact

- Email: starjw2010@gmail.com
- GitHub: https://github.com/starjw2010-cloud
- LinkedIn: https://www.linkedin.com/in/jeewon-kang-617bb7184/

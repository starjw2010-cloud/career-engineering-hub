# Public-Safe Project Inventory

This inventory summarizes local development work into recruiter-friendly categories. It intentionally avoids raw repository paths, exact private identifiers, tokens, and internal playbooks.

## Portfolio Buckets

| Bucket | Representative work | Public-safe framing | Risk level |
|---|---|---|---|
| Slack approval and request apps | Approval bot, campus decision flows, service desk flows | Slack-native workflow systems for requests, approvals, triage, and notifications | Low after ID/token removal |
| Slack operational hubs | Customer service hub, field operations hub, university operations hub | App Home dashboards with modal forms, status cards, task state, and operator views | Low after anonymization |
| Risk graph and RAG/MCP | Risk graph MCP, work memory search, campus case desk | Structured retrieval systems connecting documents, incidents, entities, and action paths | Medium; hide corpus details |
| Enterprise demo sandbox | multi-affiliate synthetic enterprise demo, portal, workflow app | End-to-end enterprise collaboration demo across Slack, portal, workflow, and RAG | Medium-high; keep high-level |
| Data safety automation | File audit bot, file gateway bot | Slack file safety workflows with scanning, review, and admin notification | Medium; hide detection rules |
| News intelligence | business news intelligence bots | Scheduled collection, categorization, deduplication, and Slack delivery | Low after source/API key removal |
| Education and enablement | Slack learning site, app studio instructions | Enablement content and reusable delivery methodology | Medium; publish summaries only |
| Frontend/product prototypes | CRM, portal, training sites | Domain-specific interface prototypes for workflow-heavy teams | Low after data cleanup |

## Recommended Public Case Studies

1. Enterprise Slack Operating System
   - Show: Slack-native workflow thinking, App Home UX, modal flows, DM confirmations, list/canvas style work tracking.
   - Hide: exact channel taxonomy, trigger IDs, org IDs, provisioning details, internal prompt library.

2. Risk Graph and RAG Workbench
   - Show: graph traversal, semantic/evidence search, MCP tools, multi-hop impact analysis.
   - Hide: full seed corpus, private entity names, exact demo queries that reveal the whole ontology.

3. Internal Portal and Workflow Hub
   - Show: FastAPI/Jinja2 portal, directory, approvals, document hub, vendor/risk dashboard, Railway deployment.
   - Hide: live internal IDs, private screenshots, exact employee/persona data.

4. File Safety and Compliance Automation
   - Show: event-driven file scanning, OCR-ready extraction, policy scoring, admin review, user notifications.
   - Hide: exact regex/rule corpus, private sample documents, workspace IDs.

5. News and Briefing Automation
   - Show: scheduled collectors, rule-based categorization, deduplication, dashboard and Slack posting.
   - Hide: API keys, private target channels, proprietary keyword sets.

## Projects Not Suitable For Direct Public Release

- Raw synthetic enterprise seed data
- Full instruction/skill folders
- Slack app manifests with real scopes and callback URLs
- Workflow trigger exports
- provisioning/identity scripts and directory-sync tooling
- Avatar/persona generation scripts and hosted asset maps
- Any `.env`, deployment logs, auth logs, or CLI output containing account context
- Internal authoring-process notes and review prompts (e.g. `codex-claude-workflow.md`, `claude-review-prompt.md`) — these encode reusable delivery strategy and may contain local paths; keep them in a private working copy, not the public repo

## Suggested Public Repo Shape

```text
career-engineering-hub/
  README.md
  docs/
    case-study-enterprise-slack-os.md
    case-study-risk-graph-rag.md
    case-study-portal-workflow.md
    case-study-file-safety.md
    project-inventory-public-safe.md
    redaction-rules.md
  site/
    index.html
    styles.css
```

Internal authoring notes (`codex-claude-workflow.md`, `claude-review-prompt.md`) are intentionally excluded from the public shape above; keep them only in a private working copy.


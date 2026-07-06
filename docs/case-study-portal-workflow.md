# Case Study: Internal Portal and Workflow Hub

## Problem

Executives and operators often need a stable web portal view even when workflow activity happens in Slack. The goal was to build a traditional internal portal that reflects the same people, approvals, documents, vendors, and risk data used by collaboration workflows.

## Role

Built the portal prototype, data loading strategy, UI templates, deployment configuration, and verification path.

## What Was Built

- server-rendered internal portal with login/session simulation
- dense enterprise-style dashboard
- employee directory and profile pages
- approvals and document views
- vendor and risk dashboards
- Slack deep-link placeholders
- bundled data snapshot for public deployment
- Docker/Railway deployment configuration

## Architecture

```text
Shared demo data
  -> data snapshot / database loader
  -> FastAPI service
  -> Jinja2 templates
  -> internal portal pages
  -> Slack/RAG context links
```

## Engineering Highlights

- intentionally avoided marketing-style UI in favor of real groupware density
- reused the same data concepts across portal, workflow, and retrieval layers
- shipped with Dockerfile, deployment config, and route health checks
- debugged deployment-specific asset loading issues after publishing

## Public-Safe Outcome

This project shows end-to-end full-stack delivery in one person's hands: data modeling, backend routes, server-rendered templates, styling, containerized deployment, and the post-deploy debugging that real launches actually require. The portal deliberately mirrors the same people, approvals, and risk data used in the Slack layer, so the two surfaces tell one consistent story.

## What Is Intentionally Omitted

- live private identifiers
- raw employee/persona data
- screenshots before redaction
- exact demo organization taxonomy


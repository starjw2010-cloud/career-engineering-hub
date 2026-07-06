# Case Study: Risk Graph and RAG Workbench

## Problem

Risk, compliance, vendor, incident, and evidence data often sits in separate places. A useful analyst tool needs to answer questions such as "what breaks if this system fails?" or "which regulation is connected to this incident?" without requiring users to manually inspect every document.

## Role

Built a synthetic graph/RAG workbench with seeded entities, relationships, documents, findings, and query tools suitable for demo and testing.

## What Was Built

- Graph-style data model for entities, systems, vendors, findings, documents, and relationships
- Hybrid retrieval that combines semantic (vector) search with graph traversal, so answers follow real relationship paths instead of keyword matches alone
- An MCP-style tool surface so an AI assistant can call the risk tools with natural-language questions
- Multi-hop impact tracing ("what breaks if this system or vendor fails?")
- Evidence document search that grounds answers in source material
- Vendor/third-party risk analysis
- Smoke tests and a demo query catalog for repeatable, reviewable results
- Deployment-ready service structure

## Architecture

```text
Documents / findings / entities
  -> seed pipeline
  -> graph database
  -> retrieval and traversal tools
  -> MCP tool responses
  -> Slack or portal presentation
```

## Engineering Highlights

- Modeled risk as connected operational context rather than isolated rows
- Combined evidence retrieval with graph traversal
- Used deterministic seed data and smoke tests to keep demos repeatable
- Documented query examples as product-facing demo scripts

## Public-Safe Outcome

This project shows I can design explainable, AI-adjacent retrieval systems: results are grounded in source documents and graph paths rather than opaque model output, and the tools are exposed cleanly enough for an assistant to consume. It reflects comfort with data modeling, retrieval design, and the practical tradeoffs of grounding an AI feature.

## What Is Intentionally Omitted

- Full synthetic corpus
- Exact ontology details that would make the demo easy to clone
- Live endpoints, internal deployment values, and private data paths


# Case Study: File Safety and Compliance Automation

## Problem

Teams often need lightweight guardrails around file sharing in collaboration tools, especially when sensitive documents can be posted into channels before review.

## Role

Designed and implemented Slack-based file audit and gateway patterns.

## What Was Built

- Event-driven file inspection flow
- Internal file download and parsing pipeline
- Support for common office/document formats and OCR-ready extraction
- Policy scoring and severity classification
- Admin review cards
- User DM notifications
- Pass/block/review workflow patterns
- Persistent audit state

## Architecture

```text
File submitted or shared
  -> app event handler
  -> secure download
  -> text extraction / OCR-ready processing
  -> policy scan
  -> admin decision or automated action
  -> user notification and audit log
```

## Engineering Highlights

- Avoided external AI APIs for sensitive content scanning
- Kept sensitive text out of Slack messages and logs
- Separated post-detection audit mode from pre-share gateway mode
- Documented operational limitations around platform permissions

## Public-Safe Outcome

This project shows security-conscious automation and sound judgment about data handling: sensitive text is deliberately kept out of messages and logs, external AI APIs are avoided for confidential content, and the design respects real platform permission limits rather than assuming ideal access. It reflects the kind of careful thinking a security- or compliance-adjacent team needs.

## What Is Intentionally Omitted

- Exact detection rule corpus
- Private sample documents
- Channel/user identifiers
- Token and permission configuration details


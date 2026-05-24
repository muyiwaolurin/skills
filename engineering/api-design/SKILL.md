---
name: api-design
description: >
  Write REST and GraphQL specs with examples. Use this skill whenever the user asks for help with
  anything related to api design. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# API Design

## Purpose

Design clear, consistent REST or GraphQL APIs. Output: spec, examples, error contracts. Users: backend engineers, tech leads, API consumers.

## Inputs to gather

- Resource domain and business operations needed
- Auth method (API key, OAuth, JWT)
- Consumers: internal service, mobile, or public third-party
- Versioning constraints and breaking vs non-breaking requirements
- Data volume and pagination needs

## Output structure

1. Resource overview - entities and relationships
2. Endpoint list - method, path, purpose, auth requirement
3. Request/response examples - JSON with realistic data
4. Error contract - status codes and error body shape
5. Versioning and deprecation notes

## Quality bar

- Every endpoint has a complete request and response example
- Error codes are specific, not generic 500s
- No ambiguous field names - use domain language consistently
- Breaking changes flagged explicitly

## Step-by-step instructions

1. Confirm resources, operations, and consumer type
2. Draft resource model - list entities and key fields
3. Map CRUD and business operations to HTTP verbs and paths
4. Design request/response shapes with all required and optional fields
5. Define error contract per endpoint
6. Add pagination, filtering, sorting where relevant
7. Flag breaking vs additive changes if modifying an existing API

## References

- `references/guide.md` - REST conventions, GraphQL patterns, OpenAPI structure

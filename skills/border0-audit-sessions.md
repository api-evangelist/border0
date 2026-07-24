---
name: Audit Border0 sessions and access activity
description: Review who accessed which resources through Border0 by pulling session logs, session stats, and organization audit actions.
api: openapi/border0-openapi.json
operations: [get_sessions, get_sessions-stats-stats-type, get_audit-actions]
---

# Audit Border0 sessions and access activity

Use this to produce an access-audit view for compliance or incident review.

## Auth
Call `https://api.border0.com/api/v1` with a Border0 service-account token (Admin or Read Only
role) in the `Authorization` header.

## Steps
1. **List sessions** — `GET /sessions` (`get_sessions`) returns sessions across the org
   (active and killed). Page through with `page` / `page_size`; filter by `socket_names`,
   `user_emails`, `start_time`, `end_time` where supported.
2. **Aggregate stats** — `GET /sessions/stats/{stats_type}`
   (`get_sessions-stats-stats-type`) rolls sessions up by `locations`, `sockets`, or `users`.
3. **Pull the audit trail** — `GET /audit/actions` (`get_audit-actions`) returns organization
   audit-log actions (who did what in the admin plane), filterable by `actor_email`,
   `resource_type`, `resource_id`.

## Notes
- Sessions can carry recordings; a socket's session recording is downloadable via the
  per-session endpoints.
- Read-only auditing needs only a Read Only service account role.
- Error envelope is `{ error_message, code }`; see `errors/border0-problem-types.yml`.

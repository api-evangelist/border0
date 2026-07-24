---
name: Create a Border0 socket and attach an access policy
description: Expose a private resource (SSH, database, HTTP, TCP) as a Border0 socket and gate it with a Zero Trust access policy.
api: openapi/border0-openapi.json
operations: [post_socket, get_socket, post_policies, get_policy-uuid, post_socket-socket-id-or-name-evaluate]
---

# Create a Border0 socket and attach an access policy

Use this to publish a protected service ("socket") in Border0 and control who can reach it.

## Auth
All calls go to `https://api.border0.com/api/v1` with a Border0 service-account token in the
`Authorization` header (securityScheme `Border0_Token`). Mint the token in the Portal
(Team > Service Accounts) or via the API. Give the service account an Admin or Member role
so it can manage resources.

## Steps
1. **Create the socket** — `POST /socket` (`post_socket`). Set the socket name and type
   (ssh, database, http, tls). The response returns the socket id/name.
2. **Confirm it exists** — `GET /socket` (`get_socket`) lists all sockets; the socket also
   resolves by id or name via `get_socket-socket-id-or-name`.
3. **Create a policy** — `POST /policies` (`post_policies`) with the policy document
   (who / when / conditions) and attach the socket(s) to it.
4. **Verify the policy** — `GET /policy/{uuid}` (`get_policy-uuid`) reads it back.
5. **Dry-run authorization** — `POST /socket/{socket_id_or_name}/evaluate`
   (`post_socket-socket-id-or-name-evaluate`) evaluates the effective policy for the socket
   before you expose it to users.

## Conventions & errors
- List endpoints paginate with `page` / `page_size`.
- Errors are `application/json` with `{ error_message, code }`; `401` = missing/invalid token,
  `403` = the identity lacks a policy/role for the action, `404` = resource not in this org.
  See `errors/border0-problem-types.yml`.

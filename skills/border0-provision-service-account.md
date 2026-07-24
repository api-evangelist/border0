---
name: Provision a Border0 service account for automation
description: Create a Border0 service account and issue an access token so CI/CD pipelines and workloads can call the Border0 admin API without human login.
api: openapi/border0-openapi.json
operations: [post_organizations-iam-service-accounts, get_organizations-iam-service-accounts, post_organizations-iam-service-accounts-name-tokens]
---

# Provision a Border0 service account for automation

Use this to give a non-human identity programmatic access to Border0.

## Auth
Call `https://api.border0.com/api/v1` with an existing admin service-account token in the
`Authorization` header. A service account's role (Admin / Member / Read Only / Client Access
Only) determines what it can manage.

## Steps
1. **Create the service account** — `POST /organizations/iam/service_accounts`
   (`post_organizations-iam-service-accounts`) with a name and role.
2. **Confirm** — `GET /organizations/iam/service_accounts`
   (`get_organizations-iam-service-accounts`) lists all service accounts in the org.
3. **Issue a token** — `POST /organizations/iam/service_accounts/{name}/tokens`
   (`post_organizations-iam-service-accounts-name-tokens`). Copy the returned token
   immediately; it is shown once. Use it as the `Authorization` value for automated calls.

## Notes
- Prefer short-lived credentials: Border0 supports Identity Federation, exchanging signed
  OIDC tokens from GitHub Actions/GitLab/CircleCI/AWS IAM for short-lived Border0 credentials,
  so pipelines avoid long-lived static tokens.
- Errors follow `{ error_message, code }`; `403` means the caller's role cannot manage IAM.
  See `conventions/border0-conventions.yml`.

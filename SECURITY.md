# Security Policy

SpendLeak's production source and security-sensitive implementation are private.

## Reporting a security issue

Please do **not** publish secrets, access tokens, private customer information, exploit details or personal data in a public GitHub issue.

Use the contact route provided on the live SpendLeak website instead:

https://spendleak.co.uk

Include enough information to reproduce or understand the issue, but minimise sensitive data.

## Public disclosure boundary

This repository intentionally excludes:

- production source code
- environment-variable and credential contracts
- database schema and privileged functions
- internal API/worker routes
- payment/provider webhook implementation
- deployment and operational workflows
- internal security runbooks
- private issue/PR history

High-level engineering and security principles may be documented publicly when doing so improves trust without weakening the production boundary.

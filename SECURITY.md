# Security Policy

## Supported Versions

The following versions of OpenTenBase receive security updates and patches:

| Version | Supported |
| ------- | --------- |
| 5.x     | Yes       |
| < 5.0   | No        |

OpenTenBase is an evolving fork derived from PostgreSQL 10 and Postgres-XL.
Security patches published by upstream PostgreSQL maintainers are evaluated
and back-ported on a best-effort basis; users on older releases should plan
an upgrade path before requesting a CVE assignment against those branches.

## Reporting a Vulnerability

**Please do not file security issues through the public GitHub issue tracker.**

OpenTenBase security disclosures follow the Tencent open-source security
response process. To report a vulnerability:

1. **Email (preferred)** -- send a detailed report to the Tencent Security
   Response Center at **security@tencent.com**.

   Please include as much of the following as you can: a concise reproducer,
   the affected commit/tag, the platform (Linux distribution, glibc version,
   CPU architecture), whether the issue is reachable without authentication,
   and any known workarounds.

2. **Encrypted communication** -- if your report is high-impact, ask for a
   PGP public key in your first email and we will reply with the disclosure
   team's current key. This is the recommended way to send exploit details
   or PoC code.

3. **GitHub Security Advisory (alternative)** -- if you prefer to stay inside
   GitHub, open a private advisory at
   <https://github.com/OpenTenBase/OpenTenBase/security/advisories/new>.
   GitHub will route it to the maintainers without disclosing the details
   publicly.

## What to Expect

| Step | Target |
| ---- | ------ |
| Acknowledge receipt | within 3 business days |
| Initial triage | within 10 business days |
| CVE request (if needed) | within 30 business days |
| Default embargo | 90 days from acknowledgment, extendable on request |

We prefer to coordinate the public release date of fixes with the reporter.

## Credit

Reporters who request it will be credited in the published advisory and in
the release notes, unless they prefer to remain anonymous.

## Out of Scope

The following are generally **not** treated as security issues for
OpenTenBase:

- Issues that require physical access to the database server.
- Denial-of-service attacks that require already-expired authentication.
- Reports against unmaintained branches (see "Supported Versions" above).
- Theoretical findings without a working exploit or concrete impact.

## Acknowledgements

The disclosure model above is adapted from the PostgreSQL Security Team
process and the Tencent open-source security response framework. We are
grateful to both communities for the ongoing work.

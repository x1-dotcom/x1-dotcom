# X1 Private Security Policy

Security reports and operationally sensitive defects must remain inside approved private X1 channels.

## Never place in issues or pull requests

Do not paste:

- passwords, API keys, tokens, private keys or signing material;
- production database contents or backups;
- customer or tenant data;
- real provider credentials;
- internal production topology that is not required for review;
- reusable exploit payloads against live X1 infrastructure.

Use sanitized identifiers, logs and reproduction data.

## Security review scope

Explicitly identify whether a change affects:

- authentication or session handling;
- authorization, RBAC or tenant isolation;
- privileged commands or remote execution paths;
- secrets, encryption or signing;
- webhook/API trust boundaries;
- package/update provenance;
- data migrations, backup/restore or destructive operations;
- audit logging and evidence integrity.

## Reporting

Use the approved private security reporting path for the repository or organization. If no dedicated path is configured, contact the X1 owner through the official internal route before transmitting sensitive evidence.

## Evidence

Separate source-level findings from reproducible tests and observed runtime behavior. Do not label a scenario production-exploitable unless that conclusion is supported by appropriate evidence.

## Remediation

Security fixes should include, where applicable, a regression test, migration/rotation plan, rollback path and an explicit statement of what remains unverified.
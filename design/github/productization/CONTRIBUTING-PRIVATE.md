# Contributing to X1 Private Engineering

This repository is part of X1 private engineering. Changes must preserve repository scope, canonical authority, tenant boundaries and operational safety.

## Before changing code

Confirm:

1. which repository or system owns the state being changed;
2. whether the change affects a public contract, data model, tenant boundary, privileged action or runtime operation;
3. what evidence exists today;
4. how the change can be rolled back safely.

Do not create a second source of truth when another X1 system is already canonical.

## Contribution rules

- Keep changes focused, reviewable and traceable.
- Preserve explicit API/event boundaries between X1 systems.
- Do not commit secrets, credentials, private keys, signing material, production databases, customer data or production dumps.
- Do not use real customer data in fixtures, screenshots, logs or tests.
- Treat schema changes, migrations, destructive operations and privileged commands as operational changes requiring rollback planning.
- Add or update tests when behavior changes.
- Update documentation when contracts, configuration, authority, deployment or operator behavior changes.
- UI changes should include current screenshots when review depends on visual behavior.

## Evidence

Use the strongest evidence actually available:

`PROVEN BY SOURCE` · `PROVEN BY TEST` · `PROVEN BY RUNTIME` · `INFERRED` · `UNKNOWN / UNPROVEN` · `RUNTIME NOT VERIFIED`

A successful build or merged pull request is not runtime proof. A configured command is not proof that a device or service consumed it.

## Pull requests

A pull request must state:

- problem and scope;
- canonical owner / authority impact;
- implementation summary;
- security, tenant and privileged-action impact;
- migration / rollback impact where applicable;
- validation performed;
- evidence level;
- remaining unknowns.

## Sensitive findings

Do not place exploit details, credentials, customer information or production topology in ordinary issues or pull requests. Follow `SECURITY.md` and use an approved private security channel.
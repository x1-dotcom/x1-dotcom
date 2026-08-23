# X1 GitHub Productization Standard

This directory defines the reusable GitHub operating layer for X1 repositories.

## Objective

Repository presentation is only one part of product quality. Every maintained X1 repository should also expose predictable contribution, security, issue-intake and pull-request workflows.

## Public baseline

Public repositories should provide:

- `CONTRIBUTING.md`
- `SECURITY.md`
- `.github/pull_request_template.md`
- `.github/ISSUE_TEMPLATE/bug.yml`
- `.github/ISSUE_TEMPLATE/feature.yml`
- `.github/ISSUE_TEMPLATE/config.yml`

The canonical public templates in this directory are:

- `CONTRIBUTING-PUBLIC.md`
- `SECURITY-PUBLIC.md`
- `PULL_REQUEST_TEMPLATE-PUBLIC.md`
- `ISSUE-BUG-PUBLIC.yml`
- `ISSUE-FEATURE-PUBLIC.yml`
- `ISSUE-CONFIG-PUBLIC.yml`

## Future-public baseline

A repository that is still private during development but has an explicit future-public target must preserve that transition boundary instead of pretending it is already public.

Use:

- `CONTRIBUTING-FUTURE-PUBLIC.md`
- `SECURITY-FUTURE-PUBLIC.md`
- `PULL_REQUEST_TEMPLATE-FUTURE-PUBLIC.md`
- `ISSUE-BUG-FUTURE-PUBLIC.yml`
- `ISSUE-FEATURE-FUTURE-PUBLIC.yml`
- `ISSUE-RELEASE-GATE-FUTURE-PUBLIC.yml`
- `ISSUE-CONFIG-FUTURE-PUBLIC.yml`
- `FUTURE-PUBLIC-RELEASE-GATE.md`

Future-public repositories should explicitly distinguish private-development-only work, code intended for publication and changes that affect a public-release gate.

## X1 evidence rule

Technical status must use evidence deliberately:

`PROVEN BY SOURCE` · `PROVEN BY TEST` · `PROVEN BY RUNTIME` · `INFERRED` · `UNKNOWN / UNPROVEN` · `RUNTIME NOT VERIFIED`

A code change, successful build or merged pull request is not automatically runtime or production proof.

## Repository boundaries

Templates must preserve the authority and legal boundary of each repository. Repositories must never request production credentials, private keys, customer data, signing material or other secrets in issues or pull requests.

Public issue intake must also keep content authorization, licensing and third-party rights explicit where the repository handles media, metadata, artwork or compatible third-party systems.

Future-public release review additionally verifies that protected X1 internals, production topology and private implementation material do not cross into the public product.

## Design principle

**ONE X1 OPERATING MODEL. REPOSITORY-SPECIFIC TRUTH.**

The workflow is standardized. Technical claims remain product-specific.

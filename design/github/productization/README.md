# X1 GitHub Productization Standard

This directory defines the reusable GitHub operating layer for X1 repositories.

## Objective

Repository presentation is only one part of product quality. Every maintained X1 repository should also expose predictable contribution, security, issue-intake and pull-request workflows.

## Public baseline

Public repositories should provide:

- `CONTRIBUTING.md`
- `SECURITY.md`
- `.github/PULL_REQUEST_TEMPLATE.md`
- `.github/ISSUE_TEMPLATE/bug_report.yml`
- `.github/ISSUE_TEMPLATE/feature_request.yml`
- `.github/ISSUE_TEMPLATE/config.yml`

## X1 evidence rule

Technical status must use evidence deliberately:

`PROVEN BY SOURCE` · `PROVEN BY TEST` · `PROVEN BY RUNTIME` · `INFERRED` · `UNKNOWN / UNPROVEN` · `RUNTIME NOT VERIFIED`

A code change, successful build or merged pull request is not automatically runtime or production proof.

## Repository boundaries

Templates must preserve the authority and legal boundary of each repository. Public repositories must never request production credentials, private keys, customer data, signing material or other secrets in issues or pull requests.

Public issue intake must also keep content authorization, licensing and third-party rights explicit where the repository handles media, metadata, artwork or compatible third-party systems.

## Design principle

**ONE X1 OPERATING MODEL. REPOSITORY-SPECIFIC TRUTH.**

The workflow is standardized. Technical claims remain product-specific.

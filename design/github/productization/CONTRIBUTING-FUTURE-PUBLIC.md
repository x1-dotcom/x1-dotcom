# Contributing to an X1 Future-Public Product

This template is for X1 repositories that remain private during development but have an explicit future-public release target.

## Before changing code

Confirm the problem, repository scope, compatibility impact and whether the change is intended to cross the future-public boundary.

Do not introduce a second authority for state owned by another X1 system. Do not couple a future public product to private X1 internals when a public contract or self-contained implementation is the correct boundary.

## Contribution rules

- Keep changes focused and reviewable.
- Preserve compatibility contracts unless a deliberate change is documented and validated.
- Keep credentials, customer/provider data, production topology, signing material and private X1 implementation details out of source, issues and pull requests.
- Treat runtime compatibility as evidence-driven, not inferred from source presence.
- Add or update tests when behavior changes.
- Update installation and compatibility documentation when required.
- Include current screenshots for meaningful UI changes.
- Confirm third-party libraries, assets and integrations are compatible with the intended public license and redistribution model.

## Evidence

Use only the strongest evidence actually available:

`PROVEN BY SOURCE` · `PROVEN BY TEST` · `PROVEN BY RUNTIME` · `INFERRED` · `UNKNOWN / UNPROVEN` · `RUNTIME NOT VERIFIED`

## Future-public boundary

Every non-trivial pull request should state whether it remains private-development-only, changes code intended for the future public product, affects a public-release gate, or introduces material requiring licensing/security review before publication.

The public release must remain useful without production credentials, customer data or protected X1 implementation details.

## Security reports

Do not post credentials or sensitive customer/provider information in issues or pull requests. Follow the repository security policy.

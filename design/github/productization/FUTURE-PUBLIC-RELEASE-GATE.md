# X1 Future-Public Release Gate

This standard applies to an X1 repository that remains private during development but is explicitly intended to become a public product.

## Mandatory review areas

A public release candidate must be reviewed for:

- repository and Git-history secret exposure;
- dependency and license compatibility;
- externally reachable security boundaries;
- credential handling and client/runtime storage behavior;
- supported runtime/device/browser validation as applicable;
- installation and configuration documentation;
- explicit public licensing;
- third-party assets/components and their redistribution/use basis;
- absence of protected X1 internals, production topology, customer/provider data and private implementation details;
- reproducible release provenance.

## Evidence rule

A checkbox, source file or successful build is not enough by itself.

Use:

`PROVEN BY SOURCE` · `PROVEN BY TEST` · `PROVEN BY RUNTIME` · `INFERRED` · `UNKNOWN / UNPROVEN` · `RUNTIME NOT VERIFIED`

`SOURCE PRESENT ≠ TESTED ≠ TARGET VERIFIED ≠ PUBLIC RELEASE READY`

## Decision states

- `BLOCKED`
- `READY FOR REVIEW`
- `APPROVED FOR PUBLIC RELEASE`
- `RELEASED PUBLIC`

No intermediate state should be presented as a completed public release.

## Boundary

A future-public X1 product should be useful within its declared public scope without requiring production credentials, private customer data or protected X1 implementation details.

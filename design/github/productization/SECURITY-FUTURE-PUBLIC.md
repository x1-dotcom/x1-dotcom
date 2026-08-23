# Security Policy — Future-Public X1 Product

This template applies to a private-development repository that is being prepared for a future public release.

## Reporting

Do not place production credentials, provider secrets, customer data, private keys, production topology or other sensitive operational material in repository content, issues or pull requests.

Use the repository's private security reporting path where available. Otherwise request a private X1 security channel through the official website before sending sensitive technical details.

Website: https://x1panel.space

## Include

When possible provide the affected commit/version, component/runtime, realistic preconditions and impact, minimal reproduction steps, sanitized evidence, release-boundary impact and mitigation ideas if known.

## Future-public security gate

Before public release, review at least repository/history secret exposure, dependencies and supply chain, externally reachable boundaries, credential handling, transport/origin assumptions and protected X1 implementation details that must not cross into the public repository.

Source-level evidence, reproducible test evidence and observed runtime behavior remain separate evidence classes.

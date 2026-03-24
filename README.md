# ARCHITECTURE

## Purpose

ARCHITECTURE defines the repository interaction map for the VERIFRAX governed system.

It describes repository roles, authority flow, execution flow, verification flow, receipt flow, and evidence registration flow.

This repository is documentation and architecture surface only.

It does not define upstream normative protocol authority.

## Repository role

- VERIFRAX authors normative source material.
- VERIFRAX-SPEC publishes derived specification artifacts from VERIFRAX.
- Derived specification artifacts are not upstream repository authority.
- Governance authority is external and bound through AUCTORISEAL plus the governed repo set in `.github`.

## Scope

This repository is responsible for:

- system topology
- repository interaction mapping
- authority and execution path documentation
- verification and evidence path documentation

This repository is not responsible for:

- authoring normative protocol semantics
- issuing authority objects
- executing governed runtime receipts
- acting as an upstream specification source

## Architecture boundary

Use this repository to understand how the governed repositories connect.

Use VERIFRAX for authored normative source material.

Use VERIFRAX-SPEC for derived publication artifacts.

Use AUCTORISEAL for authority issuance and governance-bound authority logic.

Use CORPIFORM for governed execution and receipt production.

Use VERIFRAX-verify for maintained verification surfaces.

## Current reading rule

This repository must describe current structure only.

It must not contain placeholder install instructions, fake runnable setup text, or future state written as present state.

## Contributing

See `CONTRIBUTING.md`.

## Security

Report repository questions and protocol coordination privately: **protocol@verifrax.net**

Do not open public issues for sensitive findings.

## License

Apache License 2.0. See `LICENSE`.

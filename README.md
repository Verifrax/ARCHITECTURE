# ARCHITECTURE

Topology and dependency authority map for the governed Verifrax system.

## Terminal planes

- **[ANAGNORIUM](https://github.com/Verifrax/ANAGNORIUM)** — terminal recognition
- **[REGRESSORIUM](https://github.com/Verifrax/REGRESSORIUM)** — terminal recourse

## Status

* Layer: Governance / topology reference
* Repository class: reference-only
* Package surface: none
* Public host ownership: none
* Governed role: architecture map and repository-boundary reference only
* License: Apache License Version 2.0

## One-sentence role

ARCHITECTURE defines how the Verifrax repositories, public hosts, authority surfaces, execution surfaces, verification surfaces, and evidence surfaces connect without becoming an authority, runtime, verifier, or public product surface itself.

## What this repository is

This repository is the structural map for the Verifrax stack.

It exists to describe:

* repository layer boundaries
* authority flow
* execution flow
* verification flow
* receipt flow
* evidence registration flow
* public-host ownership map
* governed dependency direction
* repository-to-surface alignment requirements

This repository is a reading surface for architecture, not a source of executable truth.

## What this repository is not

This repository is not:

* the authored protocol source
* the derived specification publication surface
* the authority issuance surface
* the governed execution runtime
* the public verifier surface
* the public proof publication surface
* the public intake surface
* the seal archive surface
* a package distribution surface
* a placeholder quickstart repository
* a generic documentation mirror

It must not contain:

* install placeholders
* fake runnable setup instructions
* speculative deployment claims
* package-install instructions for non-package content
* host claims it does not own
* authority claims it does not hold

## Authority boundary

Use this wording consistently across architecture material:

* VERIFRAX authors normative source material.
* VERIFRAX-SPEC publishes derived specification artifacts from VERIFRAX.
* Derived artifacts are not upstream authority.
* Governance authority is external and bound through AUCTORISEAL plus the governed repo set in `.github`.

ARCHITECTURE documents those relationships.
ARCHITECTURE does not create them.

## Stack position

The governed stack is modeled in this order:

1. `.github` — organization governance root and governed-repository boundary
2. `AUCTORISEAL` — authority issuance and authority reference boundary
3. `CORPIFORM` — governed execution and receipt boundary
4. `VERIFRAX` — authored protocol, evidence root, and verification boundary
5. `VERIFRAX-SPEC` — derived publication of specification artifacts
6. `VERIFRAX-PROFILES` — deterministic verification-profile corpus
7. `VERIFRAX-verify` — public verifier surface
8. `proof` — public proof publication surface
9. `apply` — public intake surface
10. `SIGILLARIUM` — seal/archive interface surface
11. `cicullis` — enforcement and merge-boundary surface

Lower layers must not be redefined by higher presentation surfaces.
Presentation repos must not silently absorb authority or execution roles.

## Public host map referenced by this repository

ARCHITECTURE owns no public host.

It must only document this host separation:

* `api.verifrax.net` — execution surface
* `proof.verifrax.net` — proof publication surface
* `auctoriseal.verifrax.net` — authority issuance/reference surface
* `corpiform.verifrax.net` — runtime reference surface
* `cicullis.verifrax.net` — enforcement reference surface
* `verify.verifrax.net` — verification tooling surface
* `sigillarium.verifrax.net` — seal/archive surface
* `apply.verifrax.net` — intake surface
* `www.verifrax.net` — commercial/public primary surface
* `verifrax.net` — apex redirect only

If any topology document collapses two of those roles into one surface without an explicit governance change, the architecture map is wrong.

## Repository reading order

Read the system in this order:

1. `.github` for governed boundary and organizational control surface
2. `AUCTORISEAL` for authority-of-record and authority artifacts
3. `CORPIFORM` for governed execution and receipt semantics
4. `VERIFRAX` for authored protocol and evidence root
5. `VERIFRAX-SPEC` for derived published specification material
6. `VERIFRAX-PROFILES` for deterministic verification profile constraints
7. `VERIFRAX-verify` for public verification surface behavior
8. `proof`, `apply`, and `SIGILLARIUM` for public-facing bounded surfaces

ARCHITECTURE should be read alongside those repos, not instead of them.

## Inputs and outputs

### Inputs

This repository consumes:

* repository role truth from governed repositories
* governance boundaries from `.github`
* authority boundaries from `AUCTORISEAL`
* execution boundaries from `CORPIFORM`
* verification and evidence boundaries from `VERIFRAX`
* derived-publication boundaries from `VERIFRAX-SPEC`
* public-surface boundaries from `VERIFRAX-verify`, `proof`, `apply`, and `SIGILLARIUM`

### Outputs

This repository produces:

* topology documentation
* stack diagrams
* dependency rules
* architecture constraints
* repository interaction references

It does not produce:

* authority objects
* execution receipts
* verifier verdicts
* evidence artifacts
* public-host deployments

## Artifact-0005 alignment requirement

This repository must remain compatible with the authority → execution → verification → evidence-registration path used by artifact-0005 in the VERIFRAX evidence root.

That means topology documents in this repository must preserve, without contradiction:

* public authority issuance through AUCTORISEAL
* governed execution through CORPIFORM
* independent verification through VERIFRAX and maintained verifier surfaces
* evidence registration in VERIFRAX

ARCHITECTURE does not register artifact-0005.
ARCHITECTURE must not claim artifact-0005 is complete, sealed, or broader than the evidence root proves.

## Canonical related repositories

* [Verifrax organization root](https://github.com/Verifrax)
* [`.github`](https://github.com/Verifrax/.github)
* [`AUCTORISEAL`](https://github.com/Verifrax/AUCTORISEAL)
* [`CORPIFORM`](https://github.com/Verifrax/CORPIFORM)
* [`VERIFRAX`](https://github.com/Verifrax/VERIFRAX)
* [`VERIFRAX-SPEC`](https://github.com/Verifrax/VERIFRAX-SPEC)
* [`VERIFRAX-PROFILES`](https://github.com/Verifrax/VERIFRAX-PROFILES)
* [`VERIFRAX-verify`](https://github.com/Verifrax/VERIFRAX-verify)
* [`proof`](https://github.com/Verifrax/proof)
* [`apply`](https://github.com/Verifrax/apply)
* [`SIGILLARIUM`](https://github.com/Verifrax/SIGILLARIUM)
* [`cicullis`](https://github.com/Verifrax/cicullis)

## CI and governance expectations

Because this repository participates in the governed documentation perimeter, it should expose real repository-identity and determinism checks where governance requires them.

The README must not use badge theater to imply checks that do not exist.

Any CI referenced here must be real, load-bearing, and mechanically verifiable.


## Verifrax system path labels

The governed Verifrax path that this README must stay compatible with is:

1. `.github` — organization governance and governed repository boundary
2. `AUCTORISEAL` — authority issuance and public authority reference
3. `CORPIFORM` — governed execution and receipt emission
4. `VERIFRAX` — authored protocol, evidence root, and artifact-chain registration boundary
5. `VERIFRAX-SPEC` — derived specification publication surface
6. `VERIFRAX-PROFILES` — deterministic profile-constraint surface
7. `VERIFRAX-SAMPLES` — pinned sample and reproducibility surface
8. `VERIFRAX-verify` — public verification repository and UI boundary
9. `VERIFRAX-DOCS` — explanatory documentation surface
10. `cicullis` — enforcement boundary
11. `proof` — proof publication surface
12. `SIGILLARIUM` — seal and archive reference surface
13. `apply` — intake surface

The live host-label map that must remain explicit and non-contradictory is:

* `https://api.verifrax.net/` — execution surface
* `https://proof.verifrax.net/` — proof publication surface
* `https://auctoriseal.verifrax.net/` — authority issuance and authority reference surface
* `https://corpiform.verifrax.net/` — runtime and receipt reference surface
* `https://cicullis.verifrax.net/` — enforcement reference surface
* `https://verify.verifrax.net/` — public verification surface
* `https://sigillarium.verifrax.net/` — seal and archive reference surface
* `https://apply.verifrax.net/` — intake surface
* `https://docs.verifrax.net/` — documentation surface

This README must remain compatible with `artifact-0005` as the load-bearing authority → execution → verification → evidence boundary without claiming that this repository alone authors, proves, seals, or registers `artifact-0005` unless that role is actually true for this repository.


## Security

Use the repository security policy for disclosure handling.

Architecture documents must not publish sensitive operational details, hidden credentials, emergency-only procedures, or private infrastructure secrets.

## Contributing

Changes to this repository change how the system is interpreted.

Accepted changes must therefore:

* preserve authority direction
* preserve host separation
* preserve repository role boundaries
* avoid speculative current-state claims
* stay aligned with governed repository truth

If a change would make a reader misidentify who owns authority, execution, verification, or public host control, the change is wrong.

## License

Apache License Version 2.0. See `LICENSE`.

## Adjacent sovereign surfaces

This repository is part of the Verifrax sovereign stack and remains bounded relative to:

- **[ANAGNORIUM](https://github.com/Verifrax/ANAGNORIUM)** for terminal recognition
- **[REGRESSORIUM](https://github.com/Verifrax/REGRESSORIUM)** for terminal recourse


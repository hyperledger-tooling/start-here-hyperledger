---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release 0.55.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.55.0
                </span>
            </td>
            <td>
                # Changelog

## [0.54.1](https://github.com/hyperledger/aries-vcx/tree/0.54.1) (2023-04-14)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.54.0...0.54.1)

### Other pull requests

- Release 0.54.1 [\#805](https://github.com/hyperledger/aries-vcx/pull/805) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Regression: Fix dependency tree when using aries\_vcx\_core [\#804](https://github.com/hyperledger/aries-vcx/pull/804) ([gmulhearn-anonyome](https://github.com/gmulhearn-anonyome))

## [0.54.0](https://github.com/hyperledger/aries-vcx/tree/0.54.0) (2023-04-13)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.53.0...0.54.0)

### Wrapper changes

- Fix node publishing [\#784](https://github.com/hyperledger/aries-vcx/pull/784) ([mirgee](https://github.com/mirgee))
- Avoid misusing peer dependencies [\#783](https://github.com/hyperledger/aries-vcx/pull/783) ([mirgee](https://github.com/mirgee))

### Refactoring

- Synchronize state machine approach [\#696](https://github.com/hyperledger/aries-vcx/issues/696)

### Other issues

- Android: vcxOpenMainPool path [\#779](https://github.com/hyperledger/aries-vcx/issues/779)

### Other pull requests

- Release 0.54.0 [\#802](https://github.com/hyperledger/aries-vcx/pull/802) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Separate core into a standalone crate [\#798](https://github.com/hyperledger/aries-vcx/pull/798) ([mirgee](https://github.com/mirgee))
- Remove unnecessary dependencies [\#796](https://github.com/hyperledger/aries-vcx/pull/796) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove proof verifier legacy format deserialization support [\#794](https://github.com/hyperledger/aries-vcx/pull/794) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Add get\_revocation\_id for IssuerCredential [\#793](https://github.com/hyperledger/aries-vcx/pull/793) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix iOS wrapper, connectionHandle [\#789](https://github.com/hyperledger/aries-vcx/pull/789) ([pomfar](https://github.com/pomfar))
- CI: Read tag 'skip-ci' to skip majority of ci jobs [\#788](https://github.com/hyperledger/aries-vcx/pull/788) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Profiles refactoring [\#785](https://github.com/hyperledger/aries-vcx/pull/785) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Bump openssl from 0.10.43 to 0.10.48 [\#782](https://github.com/hyperledger/aries-vcx/pull/782) ([dependabot[bot]](https://github.com/apps/dependabot))
- Add state machines implementation guidelines [\#781](https://github.com/hyperledger/aries-vcx/pull/781) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Vdrtools & Modular Libs as feature flags [\#763](https://github.com/hyperledger/aries-vcx/pull/763) ([gmulhearn](https://github.com/gmulhearn))
- Refactor/messages crate [\#754](https://github.com/hyperledger/aries-vcx/pull/754) ([bobozaur](https://github.com/bobozaur))

## [0.53.0](https://github.com/hyperledger/aries-vcx/tree/0.53.0) (2023-03-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.52.0...0.53.0)

### Breaking changes

- OOB invite attachment field conditional serialization, default to empty if not present [\#762](https://github.com/hyperledger/aries-vcx/pull/762) ([mirgee](https://github.com/mirgee))

### Wrapper changes

- Expose getting and clearing attributes from the ledger [\#767](https://github.com/hyperledger/aries-vcx/pull/767) ([mirgee](https://github.com/mirgee))

### Other issues

- Split libvcx, deprecate libvcx::api\_c, libvcx-ios, libvcx-java [\#753](https://github.com/hyperledger/aries-vcx/issues/753)

### Other pull requests

- Sort error mapping by numeric code [\#771](https://github.com/hyperledger/aries-vcx/pull/771) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Changed Proof \(Verifier\) API for checking presentation status [\#770](https://github.com/hyperledger/aries-vcx/pull/770) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Proof verifier: add `get_revocation_status` method [\#769](https://github.com/hyperledger/aries-vcx/pull/769) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Release 0.53.0 [\#765](https://github.com/hyperledger/aries-vcx/pull/765) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Rename prover methods, extend test test\_generate\_self\_attested\_proof [\#764](https://github.com/hyperledger/aries-vcx/pull/764) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Update nodejs in libvcx docker image to 18.14.2-r0 [\#760](https://github.com/hyperledger/aries-vcx/pull/760) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Split libvcx in 2 crates, update diagrams [\#759](https://github.com/hyperledger/aries-vcx/pull/759) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Update readme files [\#757](https://github.com/hyperledger/aries-vcx/pull/757) ([Patrik-Stas](https://github.com/Patrik-Stas))
- UniFFI Proof of Concept [\#737](https://github.com/hyperledger/aries-vcx/pull/737) ([gmulhearn](https://github.com/gmulhearn))

## [0.52.0](https://github.com/hyperledger/aries-vcx/tree/0.52.0) (2023-02-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.51.1...0.52.0)

### Wrapper changes

- Expose createServiceV2 [\#756](https://github.com/hyperledger/aries-vcx/pull/756) ([mirgee](https://github.com/mirgee))
- Expose nonmediated connection in node wrapper [\#738](https://github.com/hyperledger/aries-vcx/pull/738) ([mirgee](https://github.com/mirgee))

### Hotfixes

- Revert hiding mocking behind test\_utils feature flag [\#729](https://github.com/hyperledger/aries-vcx/pull/729) ([mirgee](https://github.com/mirgee))

### Refactoring

- Split libvcx crate [\#700](https://github.com/hyperledger/aries-vcx/issues/700)

### Other issues

- New serialization formats [\#745](https://github.com/hyperledger/aries-vcx/issues/745)
- Aries-VCX/Typestate Connection [\#740](https://github.com/hyperledger/aries-vcx/issues/740)
- Implement node FFI using napi-rs and publish node wrapper including pre-built node.js add-on [\#728](https://github.com/hyperledger/aries-vcx/issues/728)
- Move vdrtools fork under aries-vcx repo [\#724](https://github.com/hyperledger/aries-vcx/issues/724)

### Other pull requests

- Release 0.52.0 [\#758](https://github.com/hyperledger/aries-vcx/pull/758) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Rename connection 'Complete' state to 'Completed' [\#752](https://github.com/hyperledger/aries-vcx/pull/752) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix NodeJS testing CI [\#750](https://github.com/hyperledger/aries-vcx/pull/750) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Simplify connection serialization from nodejs [\#749](https://github.com/hyperledger/aries-vcx/pull/749) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix the signature of a VcxApi implementation method [\#748](https://github.com/hyperledger/aries-vcx/pull/748) ([raphaelguye](https://github.com/raphaelguye))
- Bump tokio from 1.20.3 to 1.20.4 [\#744](https://github.com/hyperledger/aries-vcx/pull/744) ([dependabot[bot]](https://github.com/apps/dependabot))
- Refactor/typestate connections [\#739](https://github.com/hyperledger/aries-vcx/pull/739) ([bobozaur](https://github.com/bobozaur))
- Remove unnecessary vdrtools code [\#736](https://github.com/hyperledger/aries-vcx/pull/736) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove generic UrsaError err mapping, handle possible UrsaErrors explicitly [\#734](https://github.com/hyperledger/aries-vcx/pull/734) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Import vdr-tools fork [\#732](https://github.com/hyperledger/aries-vcx/pull/732) ([Patrik-Stas](https://github.com/Patrik-Stas))
- CI: Do not use deprecated set-output, update artifact publishing action [\#720](https://github.com/hyperledger/aries-vcx/pull/720) ([Patrik-Stas](https://github.com/Patrik-Stas))
- CredxAnoncreds verifier functionality support [\#708](https://github.com/hyperledger/aries-vcx/pull/708) ([gmulhearn](https://github.com/gmulhearn))

## [0.51.1](https://github.com/hyperledger/aries-vcx/tree/0.51.1) (2023-01-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.51.0...0.51.1)

### Other pull requests

- Release 0.51.1 [\#727](https://github.com/hyperledger/aries-vcx/pull/727) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Update chrono dependency [\#726](https://github.com/hyperledger/aries-vcx/pull/726) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Do not bind to vdrtools FFI in ios wrapper [\#723](https://github.com/hyperledger/aries-vcx/pull/723) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.51.0](https://github.com/hyperledger/aries-vcx/tree/0.51.0) (2023-01-09)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.50.0...0.51.0)

### Breaking changes

- Remove public agent [\#715](https://github.com/hyperledger/aries-vcx/pull/715) ([mirgee](https://github.com/mirgee))

### Changes to agents

- Replace failure crate with thiserror [\#684](https://github.com/hyperledger/aries-vcx/pull/684) ([mirgee](https://github.com/mirgee))

### Refactoring

- Extract `protocols` crate [\#698](https://github.com/hyperledger/aries-vcx/issues/698)
- Simplify `messages` crate [\#697](https://github.com/hyperledger/aries-vcx/issues/697)

### Updates

- Unify Rust edition [\#693](https://github.com/hyperledger/aries-vcx/pull/693) ([mirgee](https://github.com/mirgee))

### Other issues

- Use `bs58` instead of `rust-base58` [\#694](https://github.com/hyperledger/aries-vcx/issues/694)
- Support did:key \#689 [\#690](https://github.com/hyperledger/aries-vcx/issues/690)
- Support did:key \(Aries RFC \#0360\) [\#689](https://github.com/hyperledger/aries-vcx/issues/689)

### Other pull requests

- Release 0.51.0 [\#725](https://github.com/hyperledger/aries-vcx/pull/725) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Bump tokio from 1.20.2 to 1.20.3 [\#722](https://github.com/hyperledger/aries-vcx/pull/722) ([dependabot[bot]](https://github.com/apps/dependabot))
- Improve mappings from vdrtools, refactor tests in libvcx [\#721](https://github.com/hyperledger/aries-vcx/pull/721) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Update readme.md files, update architecture diagram [\#719](https://github.com/hyperledger/aries-vcx/pull/719) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Nonmediated connection handles API [\#718](https://github.com/hyperledger/aries-vcx/pull/718) ([mirgee](https://github.com/mirgee))
- Nonmediated connection \(de\)serialization [\#717](https://github.com/hyperledger/aries-vcx/pull/717) ([mirgee](https://github.com/mirgee))
- Tweak u32 handle releasing handling [\#716](https://github.com/hyperledger/aries-vcx/pull/716) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Minor renames, remove unnecessary asyncs [\#714](https://github.com/hyperledger/aries-vcx/pull/714) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Clippy do not allow unwrap used [\#713](https://github.com/hyperledger/aries-vcx/pull/713) ([gmulhearn](https://github.com/gmulhearn))
- Libvcx/minimize api c [\#711](https://github.com/hyperledger/aries-vcx/pull/711) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Libvcx/refactor [\#710](https://github.com/hyperledger/aries-vcx/pull/710) ([Patrik-Stas](https://github.com/Patrik-Stas))
- CI: Add clippy checks [\#705](https://github.com/hyperledger/aries-vcx/pull/705) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor diddoc, extract as crate, create crate vcx\_shared [\#704](https://github.com/hyperledger/aries-vcx/pull/704) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Code formatting [\#703](https://github.com/hyperledger/aries-vcx/pull/703) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor error handling [\#702](https://github.com/hyperledger/aries-vcx/pull/702) ([Patrik-Stas](https://github.com/Patrik-Stas))
- messages: reduce dependencies, propagate errors, remove dead code [\#701](https://github.com/hyperledger/aries-vcx/pull/701) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Replace rust-base58 by bs58 [\#695](https://github.com/hyperledger/aries-vcx/pull/695) ([Patrik-Stas](https://github.com/Patrik-Stas))
- 689 support didkey aries rfc 0360 [\#691](https://github.com/hyperledger/aries-vcx/pull/691) ([guijd3p](https://github.com/guijd3p))

## [0.50.0](https://github.com/hyperledger/aries-vcx/tree/0.50.0) (2022-12-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.49.1...0.50.0)

### Other pull requests

- Release 0.50.0 [\#688](https://github.com/hyperledger/aries-vcx/pull/688) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.49.1](https://github.com/hyperledger/aries-vcx/tree/0.49.1) (2022-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.49.0...0.49.1)

### Other pull requests

- Release 0.49.1 [\#687](https://github.com/hyperledger/aries-vcx/pull/687) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix legacy wrapper ios release [\#686](https://github.com/hyperledger/aries-vcx/pull/686) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.49.0](https://github.com/hyperledger/aries-vcx/tree/0.49.0) (2022-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.48.0...0.49.0)

### Other pull requests

- Add ios legacy wrapper [\#683](https://github.com/hyperledger/aries-vcx/pull/683) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Release 0.49.0 [\#682](https://github.com/hyperledger/aries-vcx/pull/682) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.48.0](https://github.com/hyperledger/aries-vcx/tree/0.48.0) (2022-12-02)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.47.0...0.48.0)

## [0.47.0](https://github.com/hyperledger/aries-vcx/tree/0.47.0) (2022-11-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.46.0...0.47.0)

## [0.46.0](https://github.com/hyperledger/aries-vcx/tree/0.46.0) (2022-11-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.45.0...0.46.0)

## [0.45.0](https://github.com/hyperledger/aries-vcx/tree/0.45.0) (2022-11-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.44.0...0.45.0)

## [0.44.0](https://github.com/hyperledger/aries-vcx/tree/0.44.0) (2022-10-07)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.43.0...0.44.0)

## [0.43.0](https://github.com/hyperledger/aries-vcx/tree/0.43.0) (2022-10-06)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.42.0...0.43.0)

## [0.42.0](https://github.com/hyperledger/aries-vcx/tree/0.42.0) (2022-09-20)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.41.0...0.42.0)

## [0.41.0](https://github.com/hyperledger/aries-vcx/tree/0.41.0) (2022-09-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.40.0...0.41.0)

## [0.40.0](https://github.com/hyperledger/aries-vcx/tree/0.40.0) (2022-08-24)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.39.0...0.40.0)

## [0.39.0](https://github.com/hyperledger/aries-vcx/tree/0.39.0) (2022-08-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.38.0...0.39.0)

## [0.38.0](https://github.com/hyperledger/aries-vcx/tree/0.38.0) (2022-07-28)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.37.0...0.38.0)

## [0.37.0](https://github.com/hyperledger/aries-vcx/tree/0.37.0) (2022-07-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.36.0...0.37.0)

## [0.36.0](https://github.com/hyperledger/aries-vcx/tree/0.36.0) (2022-06-07)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.35.0...0.36.0)

## [0.35.0](https://github.com/hyperledger/aries-vcx/tree/0.35.0) (2022-04-13)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.34.0...0.35.0)

## [0.34.0](https://github.com/hyperledger/aries-vcx/tree/0.34.0) (2022-03-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.33.0...0.34.0)

## [0.33.0](https://github.com/hyperledger/aries-vcx/tree/0.33.0) (2022-03-02)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.32.0...0.33.0)

## [0.32.0](https://github.com/hyperledger/aries-vcx/tree/0.32.0) (2022-02-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.31.0...0.32.0)

## [0.31.0](https://github.com/hyperledger/aries-vcx/tree/0.31.0) (2022-02-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.30.0...0.31.0)

## [0.30.0](https://github.com/hyperledger/aries-vcx/tree/0.30.0) (2022-02-08)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.29.0...0.30.0)

## [0.29.0](https://github.com/hyperledger/aries-vcx/tree/0.29.0) (2022-01-26)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.28.0...0.29.0)

## [0.28.0](https://github.com/hyperledger/aries-vcx/tree/0.28.0) (2022-01-12)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.27.0...0.28.0)

## [0.27.0](https://github.com/hyperledger/aries-vcx/tree/0.27.0) (2021-12-17)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.26.0...0.27.0)

## [0.26.0](https://github.com/hyperledger/aries-vcx/tree/0.26.0) (2021-12-09)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.25.0...0.26.0)

## [0.25.0](https://github.com/hyperledger/aries-vcx/tree/0.25.0) (2021-12-06)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.24.2...0.25.0)

## [0.24.2](https://github.com/hyperledger/aries-vcx/tree/0.24.2) (2021-11-30)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.24.1...0.24.2)

## [0.24.1](https://github.com/hyperledger/aries-vcx/tree/0.24.1) (2021-11-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.23.0...0.24.1)

## [0.23.0](https://github.com/hyperledger/aries-vcx/tree/0.23.0) (2021-10-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.22.0...0.23.0)

## [0.22.0](https://github.com/hyperledger/aries-vcx/tree/0.22.0) (2021-10-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.21.0...0.22.0)

## [0.21.0](https://github.com/hyperledger/aries-vcx/tree/0.21.0) (2021-10-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.20.2...0.21.0)

## [0.20.2](https://github.com/hyperledger/aries-vcx/tree/0.20.2) (2021-09-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.20.1...0.20.2)

## [0.20.1](https://github.com/hyperledger/aries-vcx/tree/0.20.1) (2021-09-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.20.0...0.20.1)

## [0.20.0](https://github.com/hyperledger/aries-vcx/tree/0.20.0) (2021-07-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.19.0...0.20.0)

## [0.19.0](https://github.com/hyperledger/aries-vcx/tree/0.19.0) (2021-06-28)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.3...0.19.0)

## [0.18.3](https://github.com/hyperledger/aries-vcx/tree/0.18.3) (2021-06-16)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.2...0.18.3)

## [0.18.2](https://github.com/hyperledger/aries-vcx/tree/0.18.2) (2021-06-09)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.1...0.18.2)

## [0.18.1](https://github.com/hyperledger/aries-vcx/tree/0.18.1) (2021-06-03)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.0...0.18.1)

## [0.18.0](https://github.com/hyperledger/aries-vcx/tree/0.18.0) (2021-05-31)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.3...0.18.0)

## [0.17.3](https://github.com/hyperledger/aries-vcx/tree/0.17.3) (2021-04-30)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.2...0.17.3)

## [0.17.2](https://github.com/hyperledger/aries-vcx/tree/0.17.2) (2021-04-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.1...0.17.2)

## [0.17.1](https://github.com/hyperledger/aries-vcx/tree/0.17.1) (2021-03-29)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.0...0.17.1)

## [0.17.0](https://github.com/hyperledger/aries-vcx/tree/0.17.0) (2021-03-24)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.16.0...0.17.0)

## [0.16.0](https://github.com/hyperledger/aries-vcx/tree/0.16.0) (2021-01-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.15.0...0.16.0)

## [0.15.0](https://github.com/hyperledger/aries-vcx/tree/0.15.0) (2020-12-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.14.2...0.15.0)

## [0.14.2](https://github.com/hyperledger/aries-vcx/tree/0.14.2) (2020-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.14.0...0.14.2)

## [0.14.0](https://github.com/hyperledger/aries-vcx/tree/0.14.0) (2020-11-26)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.13.1...0.14.0)

## [0.13.1](https://github.com/hyperledger/aries-vcx/tree/0.13.1) (2020-11-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.13.0...0.13.1)

## [0.13.0](https://github.com/hyperledger/aries-vcx/tree/0.13.0) (2020-11-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.12.0...0.13.0)

## [0.12.0](https://github.com/hyperledger/aries-vcx/tree/0.12.0) (2020-10-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.11.0...0.12.0)

## [0.11.0](https://github.com/hyperledger/aries-vcx/tree/0.11.0) (2020-10-02)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.10.0...0.11.0)

## [0.10.0](https://github.com/hyperledger/aries-vcx/tree/0.10.0) (2020-09-24)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.9.1...0.10.0)

## [0.9.1](https://github.com/hyperledger/aries-vcx/tree/0.9.1) (2020-08-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.8.0...0.9.1)

## [0.8.0](https://github.com/hyperledger/aries-vcx/tree/0.8.0) (2020-03-31)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/d48fe2d71a839a873113890d9808c531da643288...0.8.0)




            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.55.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-04-27 04:59:34 +0000 UTC
    </span>
</div>


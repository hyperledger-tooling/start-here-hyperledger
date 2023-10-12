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
                    Release 0.60.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.60.0
                </span>
            </td>
            <td>
                # Changelog

## [0.59.1](https://github.com/hyperledger/aries-vcx/tree/0.59.1) (2023-10-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.59.0...0.59.1)

### Other pull requests

- Release 0.59.1 [\#1010](https://github.com/hyperledger/aries-vcx/pull/1010) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Use a sequence of bytes \(representing AriesMessage\) as input for EncryptionEnvelope::create [\#1007](https://github.com/hyperledger/aries-vcx/pull/1007) ([nain-F49FF806](https://github.com/nain-F49FF806))
- Do not delete target wallet, do not fail migration on item-error [\#1006](https://github.com/hyperledger/aries-vcx/pull/1006) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Add logs to credx wallet migration [\#1004](https://github.com/hyperledger/aries-vcx/pull/1004) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Use generics over trait objects in Profile & co. [\#1003](https://github.com/hyperledger/aries-vcx/pull/1003) ([bobozaur](https://github.com/bobozaur))

## [0.59.0](https://github.com/hyperledger/aries-vcx/tree/0.59.0) (2023-09-29)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.58.0...0.59.0)

### Breaking changes

- Remove msg-sending IO for issuer and holder [\#946](https://github.com/hyperledger/aries-vcx/pull/946) ([Patrik-Stas](https://github.com/Patrik-Stas))

### Hotfixes

- Fix genesis file URL in vdrproxy config [\#969](https://github.com/hyperledger/aries-vcx/pull/969) ([mirgee](https://github.com/mirgee))
- Enable compiling the workspace with --tests --all-features [\#964](https://github.com/hyperledger/aries-vcx/pull/964) ([mirgee](https://github.com/mirgee))

### Refactoring

- Integration test refactoring [\#983](https://github.com/hyperledger/aries-vcx/pull/983) ([mirgee](https://github.com/mirgee))
- Extract message sending from prover & verifier SMs [\#965](https://github.com/hyperledger/aries-vcx/pull/965) ([mirgee](https://github.com/mirgee))

### Other issues

- Remove agency\_client as dependency of integration tests [\#959](https://github.com/hyperledger/aries-vcx/issues/959)
- IO-less issuance/presentation integration tests [\#958](https://github.com/hyperledger/aries-vcx/issues/958)
- IO for prover and verifier as opt-in  [\#957](https://github.com/hyperledger/aries-vcx/issues/957)
- Add support for `names` in proof requests in `credx` anoncreds impl [\#948](https://github.com/hyperledger/aries-vcx/issues/948)

### Other pull requests

- Use standard UnpackMessageOutput struct until finally needing to transform. [\#1002](https://github.com/hyperledger/aries-vcx/pull/1002) ([nain-F49FF806](https://github.com/nain-F49FF806))
- Move CI dir [\#1001](https://github.com/hyperledger/aries-vcx/pull/1001) ([bobozaur](https://github.com/bobozaur))
- Sync up nodejs state definitions [\#999](https://github.com/hyperledger/aries-vcx/pull/999) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Add fixed nightly toolchain version for the formatting job [\#997](https://github.com/hyperledger/aries-vcx/pull/997) ([bobozaur](https://github.com/bobozaur))
- Release 0.59.0 [\#996](https://github.com/hyperledger/aries-vcx/pull/996) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix vdrproxy CI job intermittent failures [\#994](https://github.com/hyperledger/aries-vcx/pull/994) ([bobozaur](https://github.com/bobozaur))
- Added README to messages crate [\#993](https://github.com/hyperledger/aries-vcx/pull/993) ([bobozaur](https://github.com/bobozaur))
- trait\(BaseWallet\): change return type of unpack\_message, [\#992](https://github.com/hyperledger/aries-vcx/pull/992) ([nain-F49FF806](https://github.com/nain-F49FF806))
- Fix libvcx core lints [\#991](https://github.com/hyperledger/aries-vcx/pull/991) ([bobozaur](https://github.com/bobozaur))
- Issue Credential V2.0 message structures [\#990](https://github.com/hyperledger/aries-vcx/pull/990) ([gmulhearn-anonyome](https://github.com/gmulhearn-anonyome))
- Fix lints and improve formatting [\#986](https://github.com/hyperledger/aries-vcx/pull/986) ([bobozaur](https://github.com/bobozaur))
- Remove agency client from libvcx-core tests and aries-vcx-agent [\#985](https://github.com/hyperledger/aries-vcx/pull/985) ([mirgee](https://github.com/mirgee))
- Uniffi android controller [\#984](https://github.com/hyperledger/aries-vcx/pull/984) ([swaptr](https://github.com/swaptr))
- Connection protocol: add encrypt\_message, remove auto-problem-report sending [\#982](https://github.com/hyperledger/aries-vcx/pull/982) ([Patrik-Stas](https://github.com/Patrik-Stas))
- add cargo ndk build script for uniffi [\#980](https://github.com/hyperledger/aries-vcx/pull/980) ([swaptr](https://github.com/swaptr))
- Further integration test refactoring [\#979](https://github.com/hyperledger/aries-vcx/pull/979) ([mirgee](https://github.com/mirgee))
- Expose wallet migration to node wrapper [\#978](https://github.com/hyperledger/aries-vcx/pull/978) ([bobozaur](https://github.com/bobozaur))
- Remove `tokio`, `android_logger` deps from agency\_client [\#975](https://github.com/hyperledger/aries-vcx/pull/975) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Eradicate mediated connection from issuance and presentation integration tests, part 2 [\#974](https://github.com/hyperledger/aries-vcx/pull/974) ([mirgee](https://github.com/mirgee))
- Feature/msg builders [\#972](https://github.com/hyperledger/aries-vcx/pull/972) ([bobozaur](https://github.com/bobozaur))
- fix android compilation by providing libzmq to be dynamically linked [\#971](https://github.com/hyperledger/aries-vcx/pull/971) ([swaptr](https://github.com/swaptr))
- Uniffi simple message relay [\#970](https://github.com/hyperledger/aries-vcx/pull/970) ([swaptr](https://github.com/swaptr))
- Uniffi remove autogenerated bindings [\#968](https://github.com/hyperledger/aries-vcx/pull/968) ([swaptr](https://github.com/swaptr))
- Eradicate mediated connection from issuance and presentation integration tests, part 1 [\#967](https://github.com/hyperledger/aries-vcx/pull/967) ([mirgee](https://github.com/mirgee))
- Prover: fix credx credential retrieval [\#961](https://github.com/hyperledger/aries-vcx/pull/961) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix profile building in tests, considering vdrtools is default feature [\#960](https://github.com/hyperledger/aries-vcx/pull/960) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Include did:peer:3 in alsoKnownAs field in resolved DDOs [\#956](https://github.com/hyperledger/aries-vcx/pull/956) ([mirgee](https://github.com/mirgee))
- Added 'names' attribute field parsing in credx [\#955](https://github.com/hyperledger/aries-vcx/pull/955) ([bobozaur](https://github.com/bobozaur))
- Uniffi demo qr scan [\#954](https://github.com/hyperledger/aries-vcx/pull/954) ([swaptr](https://github.com/swaptr))
- Declutter issuance&presentation protocols [\#945](https://github.com/hyperledger/aries-vcx/pull/945) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove msg-sending IO from Connection protocol [\#937](https://github.com/hyperledger/aries-vcx/pull/937) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.58.0](https://github.com/hyperledger/aries-vcx/tree/0.58.0) (2023-08-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.57.1...0.58.0)

### Other issues

- Update `indy-vdr` to latest `main` \(or `0.4.0`\) [\#933](https://github.com/hyperledger/aries-vcx/issues/933)
- Reenable indy-vdr-proxy ledger tx submitter [\#930](https://github.com/hyperledger/aries-vcx/issues/930)
- Update `indy-credx` dependency to version `1.0.1` [\#926](https://github.com/hyperledger/aries-vcx/issues/926)
- Fix CI build for ios, java libvcx wrappers [\#916](https://github.com/hyperledger/aries-vcx/issues/916)

### Other pull requests

- Remove libvcx-c, libvcx java, libvcx ios [\#943](https://github.com/hyperledger/aries-vcx/pull/943) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Release 0.58.0 [\#942](https://github.com/hyperledger/aries-vcx/pull/942) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Expose public key getter on verification method [\#941](https://github.com/hyperledger/aries-vcx/pull/941) ([mirgee](https://github.com/mirgee))
- Try Hide indy-api-types from modular\_libs consumers [\#940](https://github.com/hyperledger/aries-vcx/pull/940) ([gmulhearn](https://github.com/gmulhearn))
- Extract subset of changes made in \#928 [\#939](https://github.com/hyperledger/aries-vcx/pull/939) ([mirgee](https://github.com/mirgee))
- Attempt to convert legacy DID documents to new during deserialization [\#938](https://github.com/hyperledger/aries-vcx/pull/938) ([mirgee](https://github.com/mirgee))
- Allow parsing unqualified DIDs [\#936](https://github.com/hyperledger/aries-vcx/pull/936) ([mirgee](https://github.com/mirgee))
- Update indy-vdr [\#935](https://github.com/hyperledger/aries-vcx/pull/935) ([mirgee](https://github.com/mirgee))
- Eliminate dependence of indy-ledger-response-parser on indy-api-types [\#934](https://github.com/hyperledger/aries-vcx/pull/934) ([mirgee](https://github.com/mirgee))
- Rebuild cargo.lock, restore indy-vdr-proxy txn submitter [\#932](https://github.com/hyperledger/aries-vcx/pull/932) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Updated indy-credx [\#931](https://github.com/hyperledger/aries-vcx/pull/931) ([bobozaur](https://github.com/bobozaur))
- fix\(aries-vcx\): fixed dependency listing in README for `Cargo.toml` [\#924](https://github.com/hyperledger/aries-vcx/pull/924) ([arminveres](https://github.com/arminveres))
- Refactor test setup, add interface to write DIDs on ledger [\#921](https://github.com/hyperledger/aries-vcx/pull/921) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Bump word-wrap from 1.2.3 to 1.2.5 in /wrappers/node [\#920](https://github.com/hyperledger/aries-vcx/pull/920) ([dependabot[bot]](https://github.com/apps/dependabot))
- Replace vdrtool ledger client by indy-vdr client [\#914](https://github.com/hyperledger/aries-vcx/pull/914) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Allow storing resolvers with varying extra fields in the registry [\#913](https://github.com/hyperledger/aries-vcx/pull/913) ([mirgee](https://github.com/mirgee))
- Modular did:key representation [\#912](https://github.com/hyperledger/aries-vcx/pull/912) ([mirgee](https://github.com/mirgee))
- Move PublicKey to a separate crate [\#911](https://github.com/hyperledger/aries-vcx/pull/911) ([mirgee](https://github.com/mirgee))

## [0.57.1](https://github.com/hyperledger/aries-vcx/tree/0.57.1) (2023-07-31)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.57.0...0.57.1)

### Breaking changes

- Rename tails variables in prover code [\#901](https://github.com/hyperledger/aries-vcx/pull/901) ([Patrik-Stas](https://github.com/Patrik-Stas))

### Other pull requests

- Refactor features, enable build with --no-default-features [\#918](https://github.com/hyperledger/aries-vcx/pull/918) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Release/0.57.1 [\#917](https://github.com/hyperledger/aries-vcx/pull/917) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor aries\_vcx\_core [\#910](https://github.com/hyperledger/aries-vcx/pull/910) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Specify default libvcx feature flags [\#908](https://github.com/hyperledger/aries-vcx/pull/908) ([Patrik-Stas](https://github.com/Patrik-Stas))
- testing/remove-mixed-breed [\#907](https://github.com/hyperledger/aries-vcx/pull/907) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Revert "Added capability of migrating wallet through the node.js wrap… [\#906](https://github.com/hyperledger/aries-vcx/pull/906) ([Patrik-Stas](https://github.com/Patrik-Stas))
- CI: Do not publish napi wrapper when running in fork PR [\#903](https://github.com/hyperledger/aries-vcx/pull/903) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.57.0](https://github.com/hyperledger/aries-vcx/tree/0.57.0) (2023-07-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.56.0...0.57.0)

### Other pull requests

- Release 0.57.0 [\#900](https://github.com/hyperledger/aries-vcx/pull/900) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Tweak CI to fix build-docker-android on main branch [\#899](https://github.com/hyperledger/aries-vcx/pull/899) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Cleanup/constant [\#898](https://github.com/hyperledger/aries-vcx/pull/898) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor dealing with tails\_dir in tests [\#897](https://github.com/hyperledger/aries-vcx/pull/897) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.56.0](https://github.com/hyperledger/aries-vcx/tree/0.56.0) (2023-05-23)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.55.0...0.56.0)

## [0.55.0](https://github.com/hyperledger/aries-vcx/tree/0.55.0) (2023-04-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.54.1...0.55.0)

## [0.54.1](https://github.com/hyperledger/aries-vcx/tree/0.54.1) (2023-04-14)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.54.0...0.54.1)

## [0.54.0](https://github.com/hyperledger/aries-vcx/tree/0.54.0) (2023-04-13)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.53.0...0.54.0)

## [0.53.0](https://github.com/hyperledger/aries-vcx/tree/0.53.0) (2023-03-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.52.0...0.53.0)

## [0.52.0](https://github.com/hyperledger/aries-vcx/tree/0.52.0) (2023-02-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.51.1...0.52.0)

## [0.51.1](https://github.com/hyperledger/aries-vcx/tree/0.51.1) (2023-01-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.51.0...0.51.1)

## [0.51.0](https://github.com/hyperledger/aries-vcx/tree/0.51.0) (2023-01-09)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.50.0...0.51.0)

## [0.50.0](https://github.com/hyperledger/aries-vcx/tree/0.50.0) (2022-12-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.49.1...0.50.0)

## [0.49.1](https://github.com/hyperledger/aries-vcx/tree/0.49.1) (2022-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.49.0...0.49.1)

## [0.49.0](https://github.com/hyperledger/aries-vcx/tree/0.49.0) (2022-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.48.0...0.49.0)

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
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.60.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-12 15:04:12 +0000 UTC
    </span>
</div>


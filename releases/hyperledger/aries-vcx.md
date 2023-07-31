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
                    Release 0.57.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.57.1
                </span>
            </td>
            <td>
                # Changelog

## [0.57.0](https://github.com/hyperledger/aries-vcx/tree/0.57.0) (2023-07-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.56.0...0.57.0)

### Hotfixes

- Enable compiling the workspace with --tests --all-features [\#890](https://github.com/hyperledger/aries-vcx/pull/890) ([mirgee](https://github.com/mirgee))

### Refactoring

- Remove reliance of IndyVdrLedger on global state [\#863](https://github.com/hyperledger/aries-vcx/pull/863) ([mirgee](https://github.com/mirgee))
- Split IndyVdrLedger and IndySdkLedger [\#862](https://github.com/hyperledger/aries-vcx/pull/862) ([mirgee](https://github.com/mirgee))
- Split BaseLedger trait [\#861](https://github.com/hyperledger/aries-vcx/pull/861) ([mirgee](https://github.com/mirgee))
- Remove vcx\_schema\_prepare\_for\_endorser [\#860](https://github.com/hyperledger/aries-vcx/pull/860) ([mirgee](https://github.com/mirgee))

### Other issues

- Recent versions of serde \(e.g. 1.0.167\) cause messages crate to not compile [\#893](https://github.com/hyperledger/aries-vcx/issues/893)
- Typestate Connection sends an empty string for it's publickey controller in the Invitee Request message [\#877](https://github.com/hyperledger/aries-vcx/issues/877)

### Other pull requests

- Release 0.57.0 [\#900](https://github.com/hyperledger/aries-vcx/pull/900) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Tweak CI to fix build-docker-android on main branch [\#899](https://github.com/hyperledger/aries-vcx/pull/899) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Cleanup/constant [\#898](https://github.com/hyperledger/aries-vcx/pull/898) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor dealing with tails\_dir in tests [\#897](https://github.com/hyperledger/aries-vcx/pull/897) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Update dependencies and AriesMessage Deserialize impl [\#894](https://github.com/hyperledger/aries-vcx/pull/894) ([bobozaur](https://github.com/bobozaur))
- libvcx implementation profiles [\#892](https://github.com/hyperledger/aries-vcx/pull/892) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Make PeerDid generic over numalgo [\#887](https://github.com/hyperledger/aries-vcx/pull/887) ([mirgee](https://github.com/mirgee))
- Support peer:did:3 [\#886](https://github.com/hyperledger/aries-vcx/pull/886) ([mirgee](https://github.com/mirgee))
- CI: Skip test-android job [\#885](https://github.com/hyperledger/aries-vcx/pull/885) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Implementation of did:peer:2 DID method [\#883](https://github.com/hyperledger/aries-vcx/pull/883) ([mirgee](https://github.com/mirgee))
- Remove unused lockfiles [\#882](https://github.com/hyperledger/aries-vcx/pull/882) ([mirgee](https://github.com/mirgee))
- Refactor/testing [\#880](https://github.com/hyperledger/aries-vcx/pull/880) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove unnecessary bound on DDO service [\#879](https://github.com/hyperledger/aries-vcx/pull/879) ([mirgee](https://github.com/mirgee))
- Fix 877: Connection Requests with empty DIDDoc pubkey controller [\#878](https://github.com/hyperledger/aries-vcx/pull/878) ([gmulhearn-anonyome](https://github.com/gmulhearn-anonyome))
- Fix ci [\#876](https://github.com/hyperledger/aries-vcx/pull/876) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Inject only required components, not entire profiles [\#873](https://github.com/hyperledger/aries-vcx/pull/873) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor/do not consume profile [\#872](https://github.com/hyperledger/aries-vcx/pull/872) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Sovrin-specific DDO facade [\#871](https://github.com/hyperledger/aries-vcx/pull/871) ([mirgee](https://github.com/mirgee))
- Minor DDO service builder improvement [\#868](https://github.com/hyperledger/aries-vcx/pull/868) ([mirgee](https://github.com/mirgee))
- Feature/cred migrator [\#867](https://github.com/hyperledger/aries-vcx/pull/867) ([bobozaur](https://github.com/bobozaur))
- Make DidDocument's service generic over method-specific fields [\#865](https://github.com/hyperledger/aries-vcx/pull/865) ([mirgee](https://github.com/mirgee))
- Feature/credx issuer [\#854](https://github.com/hyperledger/aries-vcx/pull/854) ([bobozaur](https://github.com/bobozaur))
- Issue \#847: Prover Handler Types [\#848](https://github.com/hyperledger/aries-vcx/pull/848) ([gmulhearn](https://github.com/gmulhearn))
- Refactor basewallet and corresponding consumers [\#843](https://github.com/hyperledger/aries-vcx/pull/843) ([tech-bash](https://github.com/tech-bash))

## [0.56.0](https://github.com/hyperledger/aries-vcx/tree/0.56.0) (2023-05-23)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.55.0...0.56.0)

### Other issues

- Consolidate transaction endorsing into a single function [\#856](https://github.com/hyperledger/aries-vcx/issues/856)
- Update dependencies of messages\_macros crate [\#846](https://github.com/hyperledger/aries-vcx/issues/846)
- Move MaybeKnown enum to shared\_vcx [\#839](https://github.com/hyperledger/aries-vcx/issues/839)
- Add ProblemReport to the IssueCredential message family [\#836](https://github.com/hyperledger/aries-vcx/issues/836)
- Add ProblemReport to the PresentProof message family [\#835](https://github.com/hyperledger/aries-vcx/issues/835)
- Move non-messages/common stuff from the messages  [\#821](https://github.com/hyperledger/aries-vcx/issues/821)
- Update `time` crate dependency to version 0.3.x [\#795](https://github.com/hyperledger/aries-vcx/issues/795)

### Other pull requests

- Release 0.56.0 [\#859](https://github.com/hyperledger/aries-vcx/pull/859) ([Patrik-Stas](https://github.com/Patrik-Stas))
- upgrade messages\_macros deps to latest [\#857](https://github.com/hyperledger/aries-vcx/pull/857) ([swaptr](https://github.com/swaptr))
- In memory response cacher [\#855](https://github.com/hyperledger/aries-vcx/pull/855) ([mirgee](https://github.com/mirgee))
- Remove dependency on BaseWallet from IndyVdrLedger [\#853](https://github.com/hyperledger/aries-vcx/pull/853) ([mirgee](https://github.com/mirgee))
- Implement txn endorsing for IndyVdrLedger [\#852](https://github.com/hyperledger/aries-vcx/pull/852) ([mirgee](https://github.com/mirgee))
- Ledger response parser [\#851](https://github.com/hyperledger/aries-vcx/pull/851) ([mirgee](https://github.com/mirgee))
- Rename crates: did\_doc\_builder-\>did\_doc; rename diddoc-\>diddoc\_legacy [\#850](https://github.com/hyperledger/aries-vcx/pull/850) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Support referrent-explicit format creating presentation request [\#844](https://github.com/hyperledger/aries-vcx/pull/844) ([Patrik-Stas](https://github.com/Patrik-Stas))
- refactor maybe\_known.rs: MaybeKnown enum [\#842](https://github.com/hyperledger/aries-vcx/pull/842) ([nachiketkanore](https://github.com/nachiketkanore))
- Fix/protocols problem report [\#840](https://github.com/hyperledger/aries-vcx/pull/840) ([bobozaur](https://github.com/bobozaur))
- Split publish\_local\_revocations in BaseAnoncreds [\#838](https://github.com/hyperledger/aries-vcx/pull/838) ([mirgee](https://github.com/mirgee))
- Add indy-vdr-proxy profile [\#837](https://github.com/hyperledger/aries-vcx/pull/837) ([mirgee](https://github.com/mirgee))
- Fix/notification problem report [\#833](https://github.com/hyperledger/aries-vcx/pull/833) ([bobozaur](https://github.com/bobozaur))
- Remove extra warn log [\#832](https://github.com/hyperledger/aries-vcx/pull/832) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Verifier presentation failure adjustments [\#830](https://github.com/hyperledger/aries-vcx/pull/830) ([bobozaur](https://github.com/bobozaur))
- Basic implementation of did:web resolver [\#828](https://github.com/hyperledger/aries-vcx/pull/828) ([mirgee](https://github.com/mirgee))
- Do not run libvcx publishing from fork PRs [\#827](https://github.com/hyperledger/aries-vcx/pull/827) ([Patrik-Stas](https://github.com/Patrik-Stas))
-  move common stuff from the messages crate to shared\_vcx [\#826](https://github.com/hyperledger/aries-vcx/pull/826) ([swaptr](https://github.com/swaptr))
- Cleanup/ffi leftovers [\#825](https://github.com/hyperledger/aries-vcx/pull/825) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix setting txn author agreement [\#824](https://github.com/hyperledger/aries-vcx/pull/824) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Refactor of the iOS CI [\#823](https://github.com/hyperledger/aries-vcx/pull/823) ([bobozaur](https://github.com/bobozaur))
- Unit test for enum SerializableObjectWithState [\#817](https://github.com/hyperledger/aries-vcx/pull/817) ([tech-bash](https://github.com/tech-bash))
- Fix README for deprecated link [\#816](https://github.com/hyperledger/aries-vcx/pull/816) ([swaptr](https://github.com/swaptr))
- Add new crates for DID parsing, DID document building, and DID resolution [\#812](https://github.com/hyperledger/aries-vcx/pull/812) ([mirgee](https://github.com/mirgee))
- unit tests for credential\_schema::Schema [\#808](https://github.com/hyperledger/aries-vcx/pull/808) ([nachiketkanore](https://github.com/nachiketkanore))
- Bump time to `0.3.20` [\#800](https://github.com/hyperledger/aries-vcx/pull/800) ([swaptr](https://github.com/swaptr))

## [0.55.0](https://github.com/hyperledger/aries-vcx/tree/0.55.0) (2023-04-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.54.1...0.55.0)

### Other pull requests

- Release 0.55.0 [\#813](https://github.com/hyperledger/aries-vcx/pull/813) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.54.1](https://github.com/hyperledger/aries-vcx/tree/0.54.1) (2023-04-14)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.54.0...0.54.1)

### Other pull requests

- Release 0.54.1 [\#805](https://github.com/hyperledger/aries-vcx/pull/805) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Regression: Fix dependency tree when using aries\_vcx\_core [\#804](https://github.com/hyperledger/aries-vcx/pull/804) ([gmulhearn-anonyome](https://github.com/gmulhearn-anonyome))

## [0.54.0](https://github.com/hyperledger/aries-vcx/tree/0.54.0) (2023-04-13)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.53.0...0.54.0)

### Other pull requests

- Release 0.54.0 [\#802](https://github.com/hyperledger/aries-vcx/pull/802) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Separate core into a standalone crate [\#798](https://github.com/hyperledger/aries-vcx/pull/798) ([mirgee](https://github.com/mirgee))
- Remove unnecessary dependencies [\#796](https://github.com/hyperledger/aries-vcx/pull/796) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove proof verifier legacy format deserialization support [\#794](https://github.com/hyperledger/aries-vcx/pull/794) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Add get\_revocation\_id for IssuerCredential [\#793](https://github.com/hyperledger/aries-vcx/pull/793) ([Patrik-Stas](https://github.com/Patrik-Stas))

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
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.57.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-07-31 11:58:50 +0000 UTC
    </span>
</div>


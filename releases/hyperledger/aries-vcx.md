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
                    Release 0.63.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.63.0
                </span>
            </td>
            <td>
                # Changelog

## [0.62.0](https://github.com/hyperledger/aries-vcx/tree/0.62.0) (2024-03-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.61.0...0.62.0)

### Bug fixes

- Publish image CI action has undeclared dependency.  [\#1140](https://github.com/hyperledger/aries-vcx/issues/1140)

### CI changes

- Fix clippy [\#1103](https://github.com/hyperledger/aries-vcx/pull/1103) ([mirgee](https://github.com/mirgee))

### Refactoring

- Remove impl\_anoncreds\_object\_identifier macro [\#1128](https://github.com/hyperledger/aries-vcx/pull/1128) ([mirgee](https://github.com/mirgee))
- refactor: remove ProofRequestData [\#1127](https://github.com/hyperledger/aries-vcx/pull/1127) ([mirgee](https://github.com/mirgee))
- refactor: ledger & anoncreds typing, part 3 [\#1124](https://github.com/hyperledger/aries-vcx/pull/1124) ([mirgee](https://github.com/mirgee))
- refactor: ledger & anoncreds typing, part 2 [\#1118](https://github.com/hyperledger/aries-vcx/pull/1118) ([mirgee](https://github.com/mirgee))
- refactor: ledger & anoncreds typing, part 1 [\#1116](https://github.com/hyperledger/aries-vcx/pull/1116) ([mirgee](https://github.com/mirgee))

### Other issues

- Retroactively address code review [\#1121](https://github.com/hyperledger/aries-vcx/issues/1121)
- Use enum as a category in RecordWallet [\#1112](https://github.com/hyperledger/aries-vcx/issues/1112)
- Remove MockWallet from release builds [\#1111](https://github.com/hyperledger/aries-vcx/issues/1111)
- Investigate and potentially remove \#!\[allow\(unused\_imports\)\]  in devsetup [\#1102](https://github.com/hyperledger/aries-vcx/issues/1102)
- Tolerance to Base64URLSafe encoding padding \(or lack thereof\) in Connection Protocol Signatures [\#1053](https://github.com/hyperledger/aries-vcx/issues/1053)
- Enable running `aries_vcx` tests in parallel [\#1050](https://github.com/hyperledger/aries-vcx/issues/1050)

### Other pull requests

- feat\(actions\): add input in publish image action and default it to ghcr.io [\#1142](https://github.com/hyperledger/aries-vcx/pull/1142) ([PanGan21](https://github.com/PanGan21))
- Release 0.62.0 [\#1141](https://github.com/hyperledger/aries-vcx/pull/1141) ([Patrik-Stas](https://github.com/Patrik-Stas))
- feat\(mediator\): Containerise and package mediator [\#1139](https://github.com/hyperledger/aries-vcx/pull/1139) ([nain-F49FF806](https://github.com/nain-F49FF806))
- feat: add packing compatibility tests [\#1138](https://github.com/hyperledger/aries-vcx/pull/1138) ([xprazak2](https://github.com/xprazak2))
- Fix running unit tests [\#1136](https://github.com/hyperledger/aries-vcx/pull/1136) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove redundant arg [\#1135](https://github.com/hyperledger/aries-vcx/pull/1135) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Improvement/derive display [\#1134](https://github.com/hyperledger/aries-vcx/pull/1134) ([Patrik-Stas](https://github.com/Patrik-Stas))
- feat: grant explicit permissions when pushing napi image [\#1133](https://github.com/hyperledger/aries-vcx/pull/1133) ([xprazak2](https://github.com/xprazak2))
- fix: push napi image using a simple command [\#1132](https://github.com/hyperledger/aries-vcx/pull/1132) ([xprazak2](https://github.com/xprazak2))
- fix: specify a tag for napi-rs image [\#1131](https://github.com/hyperledger/aries-vcx/pull/1131) ([xprazak2](https://github.com/xprazak2))
- Type requested credentials [\#1130](https://github.com/hyperledger/aries-vcx/pull/1130) ([mirgee](https://github.com/mirgee))
- feat: add workflow for building napi images [\#1129](https://github.com/hyperledger/aries-vcx/pull/1129) ([xprazak2](https://github.com/xprazak2))
- fix: use selected rust toolchain in ci [\#1126](https://github.com/hyperledger/aries-vcx/pull/1126) ([xprazak2](https://github.com/xprazak2))
- Add justfile [\#1125](https://github.com/hyperledger/aries-vcx/pull/1125) ([mirgee](https://github.com/mirgee))
- refactor: improve record category type, closes \#1112 [\#1123](https://github.com/hyperledger/aries-vcx/pull/1123) ([xprazak2](https://github.com/xprazak2))
- refactor: rename EntryTags to RecordTags [\#1120](https://github.com/hyperledger/aries-vcx/pull/1120) ([xprazak2](https://github.com/xprazak2))
- anoncreds-rs integration [\#1119](https://github.com/hyperledger/aries-vcx/pull/1119) ([mirgee](https://github.com/mirgee))
- refactor: move MockWallet to test\_utils, closes \#1111 [\#1114](https://github.com/hyperledger/aries-vcx/pull/1114) ([xprazak2](https://github.com/xprazak2))
- anoncreds-rs integration [\#1110](https://github.com/hyperledger/aries-vcx/pull/1110) ([mirgee](https://github.com/mirgee))
- refactor\(aries\_vcx\_core\): switch from derive\_builder to typed-builder [\#1108](https://github.com/hyperledger/aries-vcx/pull/1108) ([xprazak2](https://github.com/xprazak2))
- CI: Fix toolchain version [\#1107](https://github.com/hyperledger/aries-vcx/pull/1107) ([Patrik-Stas](https://github.com/Patrik-Stas))
- fix\(test\_utils\): do not ignore unused imports [\#1100](https://github.com/hyperledger/aries-vcx/pull/1100) ([xprazak2](https://github.com/xprazak2))
- DID parser using nom [\#1099](https://github.com/hyperledger/aries-vcx/pull/1099) ([mirgee](https://github.com/mirgee))
- docs: fix typos [\#1098](https://github.com/hyperledger/aries-vcx/pull/1098) ([vuittont60](https://github.com/vuittont60))
- Streamline vcxagent-core api, reformat [\#1095](https://github.com/hyperledger/aries-vcx/pull/1095) ([Patrik-Stas](https://github.com/Patrik-Stas))
- feat: replace BaseWallet with BaseWallet2 [\#1093](https://github.com/hyperledger/aries-vcx/pull/1093) ([xprazak2](https://github.com/xprazak2))
- fix: Mediated Connection - Decrypt invitation request at Invitee's as No-Auth [\#1087](https://github.com/hyperledger/aries-vcx/pull/1087) ([mkempa](https://github.com/mkempa))
- fix\(aries\_vcx\): change log msg after fn arg rename [\#1086](https://github.com/hyperledger/aries-vcx/pull/1086) ([xprazak2](https://github.com/xprazak2))
- feat: implement new wallet trait for askar [\#1085](https://github.com/hyperledger/aries-vcx/pull/1085) ([xprazak2](https://github.com/xprazak2))
- feat: add new Wallet trait, implement for indy wallet [\#1084](https://github.com/hyperledger/aries-vcx/pull/1084) ([xprazak2](https://github.com/xprazak2))
- fix: \#1053 Base64URLSafe padded and unpadded decoding [\#1083](https://github.com/hyperledger/aries-vcx/pull/1083) ([lukewli-anonyome](https://github.com/lukewli-anonyome))
- refactor: encryption envelope APIs, tests [\#1082](https://github.com/hyperledger/aries-vcx/pull/1082) ([Patrik-Stas](https://github.com/Patrik-Stas))
- fix: didcomm message forwarding [\#1081](https://github.com/hyperledger/aries-vcx/pull/1081) ([Patrik-Stas](https://github.com/Patrik-Stas))
- fix\(message\_macros\):  explicit lifetime declaration [\#1077](https://github.com/hyperledger/aries-vcx/pull/1077) ([nain-F49FF806](https://github.com/nain-F49FF806))
- fix\(mediator-client\): use standard endpoint intended for mediator clients [\#1076](https://github.com/hyperledger/aries-vcx/pull/1076) ([nain-F49FF806](https://github.com/nain-F49FF806))
- Bump openssl from 0.10.57 to 0.10.60 [\#1074](https://github.com/hyperledger/aries-vcx/pull/1074) ([dependabot[bot]](https://github.com/apps/dependabot))
- docs: Update location of aries agents [\#1073](https://github.com/hyperledger/aries-vcx/pull/1073) ([nain-F49FF806](https://github.com/nain-F49FF806))
- feat\(mediator\): Better errors for MediatorPersistence [\#1072](https://github.com/hyperledger/aries-vcx/pull/1072) ([nain-F49FF806](https://github.com/nain-F49FF806))
- refactor: encryption envelope [\#1070](https://github.com/hyperledger/aries-vcx/pull/1070) ([Patrik-Stas](https://github.com/Patrik-Stas))
- feature: Derive Display for all aries messages [\#1069](https://github.com/hyperledger/aries-vcx/pull/1069) ([Patrik-Stas](https://github.com/Patrik-Stas))
- refactor: uniffi project reorganize [\#1068](https://github.com/hyperledger/aries-vcx/pull/1068) ([swaptr](https://github.com/swaptr))
- refactor: deprecate mediation crate - include logic directly inside mediator [\#1067](https://github.com/hyperledger/aries-vcx/pull/1067) ([nain-F49FF806](https://github.com/nain-F49FF806))
- feat: Uniffi credential screen [\#1065](https://github.com/hyperledger/aries-vcx/pull/1065) ([swaptr](https://github.com/swaptr))
- chore: reorganize directory hierarchy [\#1064](https://github.com/hyperledger/aries-vcx/pull/1064) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Increase timeout in nodejs test [\#1062](https://github.com/hyperledger/aries-vcx/pull/1062) ([Patrik-Stas](https://github.com/Patrik-Stas))
- refactor: Move agents to new root \(aries\) as per \#1045 [\#1061](https://github.com/hyperledger/aries-vcx/pull/1061) ([nain-F49FF806](https://github.com/nain-F49FF806))
- Reorganize crates [\#1059](https://github.com/hyperledger/aries-vcx/pull/1059) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Uniffi demo holder [\#1058](https://github.com/hyperledger/aries-vcx/pull/1058) ([swaptr](https://github.com/swaptr))
- fix\(aries\_vcx\): make tests run in parallel [\#1057](https://github.com/hyperledger/aries-vcx/pull/1057) ([xprazak2](https://github.com/xprazak2))
- Refactor/mediator/mediation \(use integrated aries-vcx structs\) [\#1056](https://github.com/hyperledger/aries-vcx/pull/1056) ([nain-F49FF806](https://github.com/nain-F49FF806))
- Indifferent to b64url padding in indy-utils [\#1055](https://github.com/hyperledger/aries-vcx/pull/1055) ([gmulhearn-anonyome](https://github.com/gmulhearn-anonyome))
- fix\(aries\_vcx\): make integration tests run [\#1054](https://github.com/hyperledger/aries-vcx/pull/1054) ([xprazak2](https://github.com/xprazak2))
- Add mediator coordination messages to aries-vcx messages crate [\#1052](https://github.com/hyperledger/aries-vcx/pull/1052) ([nain-F49FF806](https://github.com/nain-F49FF806))
- fix\(did\_parser\): Add readme and simple example \(\#1047\) [\#1051](https://github.com/hyperledger/aries-vcx/pull/1051) ([xprazak2](https://github.com/xprazak2))

## [0.61.0](https://github.com/hyperledger/aries-vcx/tree/0.61.0) (2023-10-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.60.0...0.61.0)

## [0.60.0](https://github.com/hyperledger/aries-vcx/tree/0.60.0) (2023-10-12)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.59.1...0.60.0)

## [0.59.1](https://github.com/hyperledger/aries-vcx/tree/0.59.1) (2023-10-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.59.0...0.59.1)

## [0.59.0](https://github.com/hyperledger/aries-vcx/tree/0.59.0) (2023-09-29)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.58.0...0.59.0)

## [0.58.0](https://github.com/hyperledger/aries-vcx/tree/0.58.0) (2023-08-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.57.1...0.58.0)

## [0.57.1](https://github.com/hyperledger/aries-vcx/tree/0.57.1) (2023-07-31)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.57.0...0.57.1)

## [0.57.0](https://github.com/hyperledger/aries-vcx/tree/0.57.0) (2023-07-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.56.0...0.57.0)

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
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.63.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-17 22:28:13 +0000 UTC
    </span>
</div>


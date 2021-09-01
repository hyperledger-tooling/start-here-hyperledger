---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.1
                </span>
            </td>
            <td>
                A relatively minor maintenance release to address issues found since the 0.7.0 Release.
Includes some cleanups of JSON-LD Verifiable Credentials and Verifiable Presentations

- W3C  Verifiable Credential cleanups
  - Timezone inclusion [ISO 8601] for W3C VC and Proofs ([#1373](https://github.com/hyperledger/aries-cloudagent-python/pull/1373))
  - W3C VC handling where attachment is JSON and not Base64 encoded ([#1352](https://github.com/hyperledger/aries-cloudagent-python/pull/1352))
- Refactor outbound queue interface ([#1348](https://github.com/hyperledger/aries-cloudagent-python/pull/1348))
- Command line parameter handling for arbitrary plugins ([#1347](https://github.com/hyperledger/aries-cloudagent-python/pull/1347))
- Add an optional parameter '--ledger-socks-proxy' ([#1342](https://github.com/hyperledger/aries-cloudagent-python/pull/1342))
- OOB Protocol - CredentialOffer Support ([#1316](https://github.com/hyperledger/aries-cloudagent-python/pull/1316)), ([#1216](https://github.com/hyperledger/aries-cloudagent-python/pull/1216))
- Updated IndyCredPrecisSchema - pres_referents renamed to presentation_referents ([#1334](https://github.com/hyperledger/aries-cloudagent-python/pull/1334))
- Handle unpadded protected header in PackWireFormat::get_recipient_keys ([#1324](https://github.com/hyperledger/aries-cloudagent-python/pull/1324))
- Initial cut of OpenAPI Code Generation guidelines ([#1339](https://github.com/hyperledger/aries-cloudagent-python/pull/1339))
- Correct revocation API in credential revocation documentation ([#612](https://github.com/hyperledger/aries-cloudagent-python/pull/612))
- Documentation updates for Read-The-Docs ([#1359](https://github.com/hyperledger/aries-cloudagent-python/pull/1359),
[#1366](https://github.com/hyperledger/aries-cloudagent-python/pull/1366), [#1371](https://github.com/hyperledger/aries-cloudagent-python/pull/1371))
- Add `inject_or` method to dynamic injection framework to resolve typing ambiguity ([#1376](https://github.com/hyperledger/aries-cloudagent-python/pull/1376))
- Other fixes:
  - Indy Proof processing fix, error not raised in predicate timestamp check ([#1364](https://github.com/hyperledger/aries-cloudagent-python/pull/1364))
  - Problem Report handler for connection specific problems ([#1356](https://github.com/hyperledger/aries-cloudagent-python/pull/1356))
  - fix: error on deserializing conn record with protocol ([#1325](https://github.com/hyperledger/aries-cloudagent-python/pull/1325))
  - fix: failure to verify jsonld on non-conformant doc but vaild vmethod ([#1301](https://github.com/hyperledger/aries-cloudagent-python/pull/1301))
  - fix: allow underscore in endpoints ([#1378](https://github.com/hyperledger/aries-cloudagent-python/pull/1378))
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-08-31 23:33:49 +0000 UTC
    </span>
</div>


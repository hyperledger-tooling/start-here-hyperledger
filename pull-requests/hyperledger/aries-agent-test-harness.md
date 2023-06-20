---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    Fix acapy back channel builds.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Explicitly use python:3.7-slim-bullseye.  python:3.7-slim is now based on bookworm, and there are no Indy SDK packages for that release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 19:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/695" class=".btn">#695</a>
            </td>
            <td>
                <b>
                    ACA-Py Thread fix broke tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See ACA-Py issue [#2264](https://github.com/hyperledger/aries-cloudagent-python/issues/2264), issue [#2259](https://github.com/hyperledger/aries-cloudagent-python/issues/2259), PR [2261](https://github.com/hyperledger/aries-cloudagent-python/pull/2261)

Tested using 3 different `acapy-main`:

1. aries-cloudagent-python@main
2. aries-cloudagent-python@88769c9a3e6044ca4b22f08d83520f1553c2f97e
3. aries-cloudagent-python@0.8.2-rc0

Ran using `./manage runset acapy-aip10 -r`.

aries-cloudagent-python@0.8.2-rc0 - all tests passed, others had failures:
```
Failing scenarios:
  features/0036-issue-credential.feature:9  Issue a credential with the Holder beginning with a proposal
  features/0036-issue-credential.feature:37  Issue a credential with the Holder beginning with a proposal with negotiation
  features/0036-issue-credential.feature:66  Issue a credential with the Issuer beginning with an offer with negotiation
  features/0037-present-proof.feature:19  Present Proof where the prover does not propose a presentation of the proof and is acknowledged -- @1.1
  features/0037-present-proof.feature:20  Present Proof where the prover does not propose a presentation of the proof and is acknowledged -- @1.2
  features/0037-present-proof.feature:55  Present Proof of specific types and proof is acknowledged with a Drivers License credential type -- @1.1
  features/0037-present-proof.feature:56  Present Proof of specific types and proof is acknowledged with a Drivers License credential type -- @1.2
  features/0037-present-proof.feature:74  Present Proof of specific types and proof is acknowledged with a Biological Indicators credential type -- @1.1
  features/0037-present-proof.feature:91  Present Proof of specific types and proof is acknowledged with multiple credential types -- @1.1
  features/0037-present-proof.feature:129  Present Proof where the prover has proposed the presentation of proof in response to a presentation request and is acknowledged -- @1.1
  features/0037-present-proof.feature:130  Present Proof where the prover has proposed the presentation of proof in response to a presentation request and is acknowledged -- @1.2
  features/0037-present-proof.feature:150  Present Proof where the prover has proposed the presentation of proof from a different credential in response to a presentation request and is acknowledged -- @1.1
  features/0037-present-proof.feature:151  Present Proof where the prover has proposed the presentation of proof from a different credential in response to a presentation request and is acknowledged -- @1.2
  features/0037-present-proof.feature:207  Present Proof where the prover starts with a proposal the presentation of proof and is acknowledged -- @1.1

3 features passed, 2 failed, 9 skipped
23 scenarios passed, 14 failed, 116 skipped
193 steps passed, 14 failed, 1113 skipped, 0 undefined
Took 13m32.559s
```

The simple fix in this PR has all 3 `acapy-main` builds passing all tests. 
I have updated the BDD test code to deal with thread ids being set on credential offers.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 22:42:39 +0000 UTC
    </div>
</div>


---
layout: default
title: aries-mobile-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-test-harness
---

# aries-mobile-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-test-harness/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    working bc wallet credential offer test and agent abstraction layer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR contains a working Credential Offer test scenario using AATH based issuer. It also contains the implementation of an approach who's goal is to provide a layer of abstraction from the tests and the issuer and verifier agents to make common tests work with different issuers and verifiers. Looking mainly for review of this factory pattern approach. Please see the AGENT_ABSTRACTION.md for details.
This PR will remain in draft until I can run it with the latest BC wallet, but thought I'd get this PR started to get review on the Agent Abstraction Layer. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 00:09:28 +0000 UTC
    </div>
</div>


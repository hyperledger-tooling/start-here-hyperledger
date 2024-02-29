---
layout: default
title: aries-akrida
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-akrida
---

# aries-akrida <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-akrida){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-akrida/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Use verifier agent and config for verifier tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For the BCGov verification use cases we are using a Traction agent (just a multitenant ACA-Py really) for issuing and verifying as is done in the existing locustMediatorPresentProof test. (I'm creating my own test script that's not committed here but essentially same steps as `locustMediatorPresentProof.py`)

I'm seeing that 

1. The test invokes the issuer client to get the invite in the `get_verifier_invite` step
2. In the verifier agent web requests `load-agent/verifierAgent/acapy.py` it is using the ISSUER_* environment values instead of the VERIFIER_* ones.

I'm not sure if using a same issuer agent is the intent here? But it seems it should be using the configured verifier agent in this case instead (if that **is** to be the same agent as the issuer I think it could just be that the test operator sets the verifier config to the same url/headers as the issuer one).

I've confirmed our tests that we are developing running with the changes contained in this PR. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 00:07:15 +0000 UTC
    </div>
</div>


---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1924" class=".btn">#1924</a>
            </td>
            <td>
                <b>
                    Pre-populate revoc_reg_id on IssuerRevRegRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This avoids having a confusingly blank `revoc_reg_id` on the record in the `init` state.

Registries in the `init` state are also filtered from the `/revocation/registries/created` endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 18:15:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1922" class=".btn">#1922</a>
            </td>
            <td>
                <b>
                    fix: propagate endpoint from mediation record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves a bug in #1899 in which the public DID endpoint of an agent behind a mediator was the agent's own endpoint. These changes ensure that a mediated agent's public DID endpoint is the mediator's endpoint.

Signed-off-by: Char Howland <char@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 18:20:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1921" class=".btn">#1921</a>
            </td>
            <td>
                <b>
                    Leave credentialStatus element in the LD credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                During the implementation we stumbled upon inability of a recipient to validate a credential offer. That happens because the `credentialStatus` fields is popped from the credential offer (see [here](https://github.com/sake/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/issue_credential/v2_0/formats/ld_proof/handler.py#L506)). Later, the two entities (one from credential request, and another from the offer) are being compared, and naturally the comparison fails, which leads to inability to receive the credential offer.
This change makes sure that the comparison of the provided reference data is comparable with the credential content, by replacing the `pop` method with `get` to leave the `credentialStatus` intact in the offer object.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 12:06:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1920" class=".btn">#1920</a>
            </td>
            <td>
                <b>
                    Simple did registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This Pr simplifies the did registry to a list for future development of a did registry interface.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
Co-authored-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 17:57:58 +0000 UTC
    </div>
</div>


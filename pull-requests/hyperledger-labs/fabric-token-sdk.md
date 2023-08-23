---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    idemix aries support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This PR brings the following:
- Integrate the latest FSC version
- Simplify the idemix package for tokens by leveraging what offered by FSC
- All the integration tests use aries as backend for idemix. In the topology, this is enabled by using `dlog.WithAries(tms)`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 18:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    idemix: validate identities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This PR addresses the following issue: For the DLog driver, the identity of a token owner was not validated against the Issuer public key. This PR makes sure that this happens and that validation enforces the presence of the commitments to the EID and RH respectively. 

1. when deserializing idemix identities, check the validity of the identity and forse the presence of the nyms
2. unit-test added
3. the above is done by leveraging the latest FSC version with support for aries too.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 08:42:13 +0000 UTC
    </div>
</div>


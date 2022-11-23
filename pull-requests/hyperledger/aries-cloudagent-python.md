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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2022" class=".btn">#2022</a>
            </td>
            <td>
                <b>
                    Multi-ledger/Multi-tenant issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issues:  https://github.com/hyperledger/aries-cloudagent-python/issues/2002 and https://github.com/hyperledger/aries-cloudagent-python/issues/1989

Also fixes a couple of bugs in the alice/faber demo when running multi/multi


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 19:19:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2019" class=".btn">#2019</a>
            </td>
            <td>
                <b>
                    add isue_credential and present_proof v3 for DIDComm v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a group of university students we implemented the protocols issue_credential and present_proof for DIDComm v2. The encryption is currently still the same as for DIDComm v1.  In addition to the tests of v3, the new endpoints can be tested using a DIDComm v1 connection for now. As soon as there is a decision on how to implement/extend the existing connection for DIDComm v2, the intention is to implement it and use its information regarding the DIDComm version for choosing the encryption type (and in case of DIDComm v2 to use the encryption which is already implemented in the askar wallet).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 00:13:57 +0000 UTC
    </div>
</div>


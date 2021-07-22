---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    FABGW-21: Chaincode event listening in Node client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 17:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Add Ability to generate HSM identities for Scenario tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note that this explicitly disables TLS only for the CAs. 
If TLS remains enabled then it becomes a problem as the fabric-ca-client will try to verify using the CA Cert and you then need to interact with the CA using the url ca.org1.example.com which cannot be resolved outside of the docker network without modifying /etc/hosts (which is messy).
fabric-ca-client inside the CA container doesn't have access to the pkcs11 library and you can't just mount it in because the CA Container is built around alpine which uses a different C runtime.
Disabling TLS for the CAs solves this problem and is not detrimental to the testing of fabric-gateway

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 08:22:09 +0000 UTC
    </div>
</div>


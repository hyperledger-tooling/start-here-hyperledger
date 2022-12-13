---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    added a check for prereq into deploycc script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a check for prerequisites into deployCC script.  
Issue: https://github.com/hyperledger/fabric/issues/3848

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 13:51:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/883" class=".btn">#883</a>
            </td>
            <td>
                <b>
                    Parse transaction creator to Identity in off_chain_data samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Parsing out of the creator / signer information to provide direct access to their X.509 certificate supports this end-user StackOverflow question:

https://stackoverflow.com/questions/74718400/get-clients-signature-from-the-hyperledger-fabric-block-and-verify-it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 11:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    Update org1-peer2.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixing TLS issues while using org1-peer-gateway-svc.${DOMAIN}. This would be needed so there are no TLS issues when sending requests.

Signed-off-by: Deepak Singh <91736795+blockguardian@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 18:40:36 +0000 UTC
    </div>
</div>


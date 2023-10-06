---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1415" class=".btn">#1415</a>
            </td>
            <td>
                <b>
                    feature: changes to support upgrade to Fabric v2.5 TLS in Firefly CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Updated GO to version 1.20 (Fabric 2.5 compatibility) and Ubuntu as the base instead of Alpine.
 
 Fixes this Issue: #1414 
 
 Related to the Firefly CLI change here: #https://github.com/hyperledger/firefly-cli/issues/268
 
 E2E test passed:
 
 --- PASS: TestFabricMultipartyE2ESuite (137.02s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EBroadcast (3.97s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EBroadcastBlob (34.51s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EPrivate (3.74s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EPrivateBlobDatatypeTagged (3.71s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EWebhookExchange (7.61s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EWebhookRequestReplyNoTx (4.78s)
    --- PASS: TestFabricMultipartyE2ESuite/TestStrongDatatypesBroadcast (7.58s)
    --- PASS: TestFabricMultipartyE2ESuite/TestStrongDatatypesPrivate (7.29s)
    --- PASS: TestFabricMultipartyE2ESuite/TestCustomChildIdentityBroadcasts (7.88s)
    --- PASS: TestFabricMultipartyE2ESuite/TestCustomChildIdentityPrivate (11.26s)
    --- PASS: TestFabricMultipartyE2ESuite/TestInvalidIdentityAlreadyRegistered (9.39s)
    --- PASS: TestFabricMultipartyE2ESuite/TestE2EContractEvents (2.69s)
PASS
ok  	github.com/hyperledger/firefly/test/e2e/runners	137.028s
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 11:52:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1413" class=".btn">#1413</a>
            </td>
            <td>
                <b>
                    Add docs for AND/OR option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See detail in https://github.com/hyperledger/firefly-common/pull/71
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 20:42:51 +0000 UTC
    </div>
</div>


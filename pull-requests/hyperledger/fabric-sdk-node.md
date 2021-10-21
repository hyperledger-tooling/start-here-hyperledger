---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/522" class=".btn">#522</a>
            </td>
            <td>
                <b>
                    [refactor] ServiceHandler.js->function type ServiceHandler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It might involve
- rewrite DiscoveryHandler.js
- migrate to use TargetedHandler.js
- more code hygiene in Proposal.js
- more use subclass of Proposal.js, than ServiceAction

Signed-off-by: DavidLiu <david.yx.liu@oracle.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 09:58:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/519" class=".btn">#519</a>
            </td>
            <td>
                <b>
                    Publish Contract JSDoc (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was being excluded from the generated JavaScript files as it was not immediately above a class definition that would be written to the JavaScript file by the TypeScript compiler.

Also add the TransactionError as a possible thrown exception from Transaction.submit().

Contributes to #504 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 13:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/518" class=".btn">#518</a>
            </td>
            <td>
                <b>
                    Publish Contract JSDoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was being excluded from the generated JavaScript files as it was not immediately above a class definition that would be written to the JavaScript file by the TypeScript compiler.

Also add the TransactionError as a possible thrown exception from Transaction.submit().

Resolves #504 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 13:46:54 +0000 UTC
    </div>
</div>


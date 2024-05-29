---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/578" class=".btn">#578</a>
            </td>
            <td>
                <b>
                    ci scripts update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-29 14:07:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    update HLE and samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                This PR does the following:
- It updates HLE docker images to version 2.0 (https://github.com/hyperledger-labs/blockchain-explorer)
- Updates to the samples
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-29 08:52:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/576" class=".btn">#576</a>
            </td>
            <td>
                <b>
                    Align DB naming
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 14:23:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/574" class=".btn">#574</a>
            </td>
            <td>
                <b>
                    Cache fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses two issues detected by the integration tests of Token SDK:
* When two nodes try to set the state at the same time, one gets a duplicate error and doesn't update the vault. Then we don't fail, because we know that another process has updated it, but the txidstore cache remains with the same previous value. Now we invalidate the cache and fetch the new value.
* When multiple replicas are trying to commit the same TX and rewrite the same keys, we get a deadlock error from the DB. Now we retry every time we get a deadlock error until the operation is successful. This means that either the other writes have failed so we can write the new values, or the other writes were successful so we update the state (using the same values).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 06:45:04 +0000 UTC
    </div>
</div>


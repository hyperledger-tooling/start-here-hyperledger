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
                PR <a href="https://github.com/hyperledger/firefly/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    add E2E test for token plugins with remote names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                in a chain with #919 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 22:11:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    E2E test for tokens only namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                * Adds an E2E test for namespaces with only a `tokens` plugin
* Moves `keynormalization` config under `namespaces.predefined[].assets.manager.keynormalization`
* Adds common for code adding namespaces, resetting firefly, etc. to a common package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 18:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    Add multi-tenancy E2E test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a chain with #916

Includes additional fixes for separating messages/data on different namespaces.

This also includes changes to the NextPins table to add a namespace column.
While it's not possible to populate namespace on any existing entries, we make a best
effort at migration by setting the namespace every time a row is updated. This will allow
legacy environments to migrate over time, as long as they don't immediately add
multi-tenant nodes alongside existing ones.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 17:55:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Add admin and config fields to E2E testState
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
        Created At 2022-08-02 12:57:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/916" class=".btn">#916</a>
            </td>
            <td>
                <b>
                    Add node-specific suffix to DX endpoint "id"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~In a chain with #915~~
Depends on https://github.com/hyperledger/firefly-dataexchange-https/pull/62

UPDATE: found a number of bugs while adding E2E tests - so #918 contains everything from this PR, some additional fixes, and an E2E test. The comments below are still relevant though.

FireFly can now support many local namespaces that map to a single remote namespace (for multi-tenancy purposes). Each of these local namespaces may have their own "node" within FireFly, but they may all be sharing a single DX plugin. This change adds a "nodeName" qualifier to many of the dataexchange plugin calls, along with a specific implementation in the FFDX plugin code, to allow many nodes to exist behind a single DX.

Implementation outline:
* For newly created nodes, the FFDX connector will append a suffix to the member ID advertised by the plugin before storing or broadcasting it. This means each node will have a unique verifier ID even if they are sharing a DX member ID and certificate. The FFDX connector and FFDX plugin have agreed on `/` as a separator.
* The FFDX connector will ignore this suffix when routing messages (paying attention only to the member ID before the separator) - but will pass the full recipient string for further routing by FireFly on the far end.
* FireFly will use the combination of the received message's remote namespace and recipient ID to route it uniquely to a single event manager.

Should remain fully backwards compatible for nodes that were already broadcast/stored in the database with a non-suffixed peer ID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 17:44:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/915" class=".btn">#915</a>
            </td>
            <td>
                <b>
                    Allow multiple copies of things on different namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Everything that can be sent (messages, data, all definition types) needs to only be unique within a namespace. The IDs can no longer be considered globally unique, and the database needs to reflect that.

Move "node" configuration to the "multiparty" section (next to "org"), as different namespaces may want to advertise different names for their local node.

Clean up operation handling in DX to make it consistent with other plugins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-30 17:35:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/914" class=".btn">#914</a>
            </td>
            <td>
                <b>
                    Fix test coverage gaps in operations manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduced by #911
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 13:44:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    Use "poolData" instead of "namespace" in fftokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on:
https://github.com/hyperledger/firefly-tokens-erc1155/pull/84
https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/70
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 21:51:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/912" class=".btn">#912</a>
            </td>
            <td>
                <b>
                    Update UI version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                UI is fully functional again with latest mainline code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 17:56:06 +0000 UTC
    </div>
</div>


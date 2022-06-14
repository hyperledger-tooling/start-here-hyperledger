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
                PR <a href="https://github.com/hyperledger/firefly/pull/858" class=".btn">#858</a>
            </td>
            <td>
                <b>
                    Remove redundant payloadRef field on Batch Pin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This field is not used by any code.

There was a vision that storing the `payloadRef` on broadcast batches for reference, but this was never implementing. Meaning this field is cruft.

Currently the right way to find the payload reference, is to look at the upload/download operations for the batch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 15:29:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/857" class=".btn">#857</a>
            </td>
            <td>
                <b>
                    FAQ and FireFly Tutorial Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two main changes in this PR:
1- FAQ updates. Added some FAQs related to deploying smart contracts, connecting to Metamask, and how FireFly enables multi-chain applications
2- FireFly tutorial updates. Fixed some links to swagger pages that were outdated, updated some instructions, added instructions and screenshots on using the FireFly sandbox in order to follow along some of the examples given in the tutorials
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 17:19:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/856" class=".btn">#856</a>
            </td>
            <td>
                <b>
                    Add namespace to pins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Existing pins will all be categorized against "ff_system", just so the field has a non-null value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 16:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    Use a separate orchestrator for each namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed in this PR:
- Namespace manager is now the root manager in the system
- There is a separate orchestrator for each namespace, along with a separate instance of (almost) every manager
- Config for including different plugins in each namespace is now honored
- Each plugin supports multiple listeners, and each listener function (mostly on event manager) will filter out events from just the one namespace to which it's assigned

Broken in this PR:
- You cannot have multiple namespaces that point at the same blockchain FireFly contract, or the same token pool. They will end up sharing an event stream and therefore only one of them will process events. Fixing this will require splitting a lot of the contract/event stream logic out of the blockchain plugins into a new per-namespace component.
- Performance of event processing degrades almost linearly with the number of created namespaces, due to the fact that most events are fired to _all_ instances of the event manager and then examined in order to process or ignore them. In the future, we can push namespace knowledge down into lower layers to make this decision earlier and avoid this extra overhead.
- SPI route for "get all operations" is completely broken. This needs a redesign with how FFTM functions.

~~Also includes the changes from #856.~~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 01:36:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/854" class=".btn">#854</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the link to the Contributors link which was broken before 
https://hyperledger.github.io/firefly/contributors/

Signed-off-by: viswatejagajulavarthy <67342185+viswatejagajulavarthy@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 17:35:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/853" class=".btn">#853</a>
            </td>
            <td>
                <b>
                    Restore FireFly contract version, update UI version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor fixes to stabilize main ahead of the next alpha release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 14:50:09 +0000 UTC
    </div>
</div>


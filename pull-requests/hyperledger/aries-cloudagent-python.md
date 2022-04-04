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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1706" class=".btn">#1706</a>
            </td>
            <td>
                <b>
                    Multitenancy Docs Update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Please review the updates to the multitenancy docs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 17:01:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1705" class=".btn">#1705</a>
            </td>
            <td>
                <b>
                    Fix Issue-1682
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added wallet startup parameter: --wallet-allow-insecure-seed
- support seed in wallet/did/create route

Some questions around
1. How do we support importing a key pair into the wallet as mentioned in the Issue
2. Should I add seed in the schema of wallet/did/create ? . I don't think we can add conditional schemas according to startup parameter.  I can have it as an optional field.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 10:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1702" class=".btn">#1702</a>
            </td>
            <td>
                <b>
                    Add auto_verify flag in present-proof protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: DaevMithran <daevmithran1999@gmail.com>

Fix [https://github.com/hyperledger/aries-cloudagent-python/issues/1698](url)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 12:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1701" class=".btn">#1701</a>
            </td>
            <td>
                <b>
                    Allow deleting a pres exchange item without reading it first
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to #1687 this allows deleting a presentation exchange
record without reading it from storage.

@shaangill025 Does it make sense to have something like this in addition to your change in #1690 to make sure we always have an option to delete an item without reading it?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 11:30:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1700" class=".btn">#1700</a>
            </td>
            <td>
                <b>
                    Fix: update IndyLedgerRequestsExecutor logic - multitenancy and basic base wallet type 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1691 
- Earlier `IndyLedgerRequestsExecutor` instance was retrieved by calling `profile.inject(IndyLedgerRequestsExecutor)` which would correspond to the `root_profile`. If the base `wallet_type` is basic then the `BaseLedger` instance will not be specified which caused the above issue. I have now updated the logic to create a new `IndyLedgerRequestsExecutor` instance for each sub wallet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 23:09:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1697" class=".btn">#1697</a>
            </td>
            <td>
                <b>
                    platform target in run tests.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @dbluhm suggested seeing if adding a platform target would allow docker to run the test scripts, which worked. I expect more changes for complete mac m1 development support but this seems to be a good starting point.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 22:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1696" class=".btn">#1696</a>
            </td>
            <td>
                <b>
                    Endorser support for updating DID endpoints on ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                As stated in #1447, the changes by Harsh fix an issue where ACA-Py could not publish ATTRIB records because they were not signed by the endorser. We need those changes in for 0.7.4 if possible, but PR #1616 has not seen any updates and has merge conflicts with the latest changes in main. I have attempted to fix those merge conflicts and make the requested changes from @ianco in that PR, as well as fix all the unit test failures. 

This closes #1616. I am not sure if more work is needed for #1447.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 22:08:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1694" class=".btn">#1694</a>
            </td>
            <td>
                <b>
                    Feature/undelivered events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds in a number of events which are emitted when a message is undelivered.

These events can be leveraged by plugins to take certain actions when messages are undelivered, such as writing the message to a persistent queue, sending a push notification to a mobile device that attempted to send the message, or some other action.

The events leverage the existing `OutboundSendStatus` states and don’t supersede the current return value. The `OutboundSendStatus` is still returned within ACA-Py as it has been, so this shouldn’t impact any existing functionality, but I’d be happy to hear any concerns I’ve not thought of. Thanks to @dbluhm for his feedback prior to this PR being opened. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 19:07:09 +0000 UTC
    </div>
</div>


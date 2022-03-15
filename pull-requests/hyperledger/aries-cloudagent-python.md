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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1668" class=".btn">#1668</a>
            </td>
            <td>
                <b>
                    Fetch stored credentials prior to sending ack response in issue-credential 2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attempt to fix an issue with blank credential values seen in the test harness.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 22:35:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1667" class=".btn">#1667</a>
            </td>
            <td>
                <b>
                    Fix: present-proof v2 send-proposal [issue#1474]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>

resolve #1474 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 16:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1665" class=".btn">#1665</a>
            </td>
            <td>
                <b>
                    fix: always notify if revocation notification record exists
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes the check to notify in the `on_revocation_published` event handler. This check in the `on_revocation_published` would only take the global config option into account, meaning it doesn't matter if you provided `notify: true` in the `/revoke` endpoint.

A`RevNotificationRecord` is only created if a notification should be sent (either global agent config, or `notify` prop in the revoke endpoint). So if a record exists I think we can assume that a notification should be sent as otherwise the record wouldn't exist in the first place. Maybe I'm missing something?

https://github.com/hyperledger/aries-cloudagent-python/blob/681e9aab9a6f6d3e76484d02ccb969d3227bf34f/aries_cloudagent/revocation/manager.py#L116-L126


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 19:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1663" class=".btn">#1663</a>
            </td>
            <td>
                <b>
                    Add "sent" key to both Schema and Cred Defs when using Endorsers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As an Author, if I attempt to publish duplicate schemas or credential definitions, I get a trace stack returned to me complaining about how the `signed_txn` key does not exist. While I adding a response for that situation (to just return the schema ID/ Cred Def ID instead of an error), I noticed that we were never populating the `"sent"` key in our responses to controllers. I have standardized the responses to follow the OpenAPI Schema and included the `"sent"` key.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 18:41:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1660" class=".btn">#1660</a>
            </td>
            <td>
                <b>
                    Revert change to send_credential_ack return value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to #1619 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 23:52:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1659" class=".btn">#1659</a>
            </td>
            <td>
                <b>
                    Redis PQ Cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 17:04:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1658" class=".btn">#1658</a>
            </td>
            <td>
                <b>
                    [RFC] Do NOT merge yet - Allow access to /ledger/register-nym with multitenancy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The change shows what might be necessary to support "Option 3" described in #1657 

Still needs discussion whether this is the desired way to go.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 14:33:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1655" class=".btn">#1655</a>
            </td>
            <td>
                <b>
                    Add cred_def_id to metadata when using an Endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When publishing a new credential definition to the ledger (with the Author/Endorser workflow), the `cred_def_id` is nowhere to be found in the transaction response or the webhooks. I have moved the metadata definition lines for `cred_def_id` and `issuer_id` to the actual definition point for the metadata and have removed the redundant lines that were in an if block.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 16:47:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1654" class=".btn">#1654</a>
            </td>
            <td>
                <b>
                    docs: supported features attribution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also updates the rocket chat link to a discord link

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 08:43:38 +0000 UTC
    </div>
</div>


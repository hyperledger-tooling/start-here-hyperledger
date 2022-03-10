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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1653" class=".btn">#1653</a>
            </td>
            <td>
                <b>
                    Fix usage of send_credential_ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow up to #1619
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-05 00:35:17 +0000 UTC
    </div>
</div>


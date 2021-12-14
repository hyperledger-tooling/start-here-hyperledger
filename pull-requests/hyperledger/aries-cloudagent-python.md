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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1558" class=".btn">#1558</a>
            </td>
            <td>
                <b>
                    Await asyncio.sleeps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a few warnings during tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 22:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1557" class=".btn">#1557</a>
            </td>
            <td>
                <b>
                    ACA-Py Upgrade command implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 17:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1556" class=".btn">#1556</a>
            </td>
            <td>
                <b>
                    Added event queue support as an alternative to webhook notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## What is this PR for?

- Added external queue support as an alternative to HTTP webhook events
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 14:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1553" class=".btn">#1553</a>
            </td>
            <td>
                <b>
                    PR#1543 Follow up - Adding invitation_msg_id and their_public_did back to record_value.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 20:13:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1551" class=".btn">#1551</a>
            </td>
            <td>
                <b>
                    Update demo requirements
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
        Created At 2021-12-11 00:45:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1550" class=".btn">#1550</a>
            </td>
            <td>
                <b>
                    Remove required dependencies from multi-ledger code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also adjusts the return value from `get_ledger_for_identifier` for consistency.

Fixes #1549 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 23:55:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1545" class=".btn">#1545</a>
            </td>
            <td>
                <b>
                    Add credential_revoked state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pull request for [Issue: 1539](https://github.com/hyperledger/aries-cloudagent-python/issues/1539)
@swcurran  Added the credential_revoked state. 
For now I have considered only issue-credential 1.0, I should check for the record in V20CredentialExchange too.
Will do it soon. If you have any suggestions on my approach please comment below.

Questions:
- Is it required raise an error if the credential record doesn't exist? 
- The credential state should be changed only after publishing revocation.
   When publish is set to pending, what is the best way to implement this?. I'm planning to create retrieve credential records using rev_reg_id and cred_rev_id
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 09:28:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    Remove request_id from inviter connection record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issue https://github.com/hyperledger/aries-cloudagent-python/issues/1541

Tested in alice/faber, there are some error messages on the faber side however the connection (didexchange) is established and can be used for issuing credentials and requesting proofs.

Not sure what is the issue of removing `request_id` from the inviter connection record, or why it's required for didexchange but not connections protocol.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 19:27:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1543" class=".btn">#1543</a>
            </td>
            <td>
                <b>
                    ConnRecord tags - `their_public_did` and `invitation_msg_id`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
- resolve #1542 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 19:18:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1538" class=".btn">#1538</a>
            </td>
            <td>
                <b>
                    Fix validation for range checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 02:11:45 +0000 UTC
    </div>
</div>


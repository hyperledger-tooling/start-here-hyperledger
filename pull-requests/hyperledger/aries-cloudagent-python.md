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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1210" class=".btn">#1210</a>
            </td>
            <td>
                <b>
                    BUG FIX: set connections metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Due https://github.com/hyperledger/aries-cloudagent-python/pull/1186#issuecomment-849452360 

There was a bug that does not save the metadata into the records once they were set.
This PR fixes that bug, updating the connections metadata everywhere.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 11:25:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1209" class=".btn">#1209</a>
            </td>
            <td>
                <b>
                    Fix exposing wallet storage creds in configuration endpoint.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #1208 

Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 09:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1207" class=".btn">#1207</a>
            </td>
            <td>
                <b>
                    Fix message types of problem report 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Similar fix with https://github.com/hyperledger/aries-cloudagent-python/pull/1190
Thanks!

@sklump 

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 07:47:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1204" class=".btn">#1204</a>
            </td>
            <td>
                <b>
                    Fix: Public Connections Invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1203 
- Went through the following test cases, all invitations should now work as expected.
![image](https://user-images.githubusercontent.com/9292265/119702684-942f2480-be0a-11eb-9527-cbff0e26f885.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 17:11:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1202" class=".btn">#1202</a>
            </td>
            <td>
                <b>
                    Updates to OOB InvitationMessage & Endpoint example - Consistent with RFC0434
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1138 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 11:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1200" class=".btn">#1200</a>
            </td>
            <td>
                <b>
                    Changes in Endorser Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request consists of the following changes in endorser protocol : 

1.  The author can give the functionality to the endorser where he/she can auto-write the transaction to the ledger after it gets endorsed.
2. The agent from where the transaction is written to the ledger is separated, it the author writes the transaction, it would go from author's agent and same for endorser.
3. Always, the record would be stored in author's wallet, irrespective of who (Author/Endorser) actually writes the transaction to the ledger.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-22 19:12:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1199" class=".btn">#1199</a>
            </td>
            <td>
                <b>
                    fix cascading problem report, error state failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sorry about that
Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 21:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1197" class=".btn">#1197</a>
            </td>
            <td>
                <b>
                    Changed retrieve_tails to delete invalid tails files after fetching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove downloaded tails files with invalid hashes. This fixes #1196
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 14:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1195" class=".btn">#1195</a>
            </td>
            <td>
                <b>
                    Mitigate rich schema thirst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix protocols/problem_report/v1_0/__init__.py internal_error() en passant: hadn't been creating compliant RFC 35 ProblemReport objects, resulting in cascading failure
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 13:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1193" class=".btn">#1193</a>
            </td>
            <td>
                <b>
                    Fix: OOB Invitation against Public DIDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Now able to create and receive OOB invitations against public DIDs.
- Fixes not being able to load `IndyDIDResolver`.
- Implement `supported_did_regex` in `KeyDIDResolver` and `IndyDIDResolver`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 09:08:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    Fix bug with problem report 2.0 handler and message family
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a bug caused by inconsistent naming that would result in problem reports not being handled correctly by the receiving agent for `issue-credential-2.0`.

I am surprised all the unit tests passed before: is there a testing pattern I should be looking into to add one, or is this something that will/should be caught by the test harness?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 20:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    AIP-2 base64url consistency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - In regards to decoding, we handle base64 permissively, passing `urlsafe` as `True`.
- If `emit_new_didcomm_mime_type` and `emit_new_didcomm_prefix` arguments are set, send everything as base64url [updates `data_base64` accordingly] else leave eveything as it is.
closes #1108
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 16:22:29 +0000 UTC
    </div>
</div>


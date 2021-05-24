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
                - Pending approval and merge of #1193 
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    Tags on connection metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With this PR, It is possible to add tags to connections. The tags are saved as a metadata key-value on the connections record.
Once the connections have been tagged, it is possible to group them on tags.

The tags are added on `/connections/create-invitation` & `/connections/receive-invitation` via a query parameter called `tags` in the request.  The input is a string, it is possible to add multiple tags if they are separated by commas. 

The tags could be filtered on `/connections` via a query parameter called `tags` in the request. The input is a string, it is possible to filter by multiple tags if they are separated by commas.

**Examples**:

- Create invitation

> Request
`curl -X POST "http://localhost:8021/connections/create-invitation?tags=tag1%2Ctag3" -H "accept: application/json" -H "Content-Type: application/json" -d "{ }"`

> Response
`{
  "connection_id": "8e1d9605-5843-4844-99d1-96141329e006",
  "invitation": {
    "@type": "did:sov:BzCbsNYhMrjHiqZDTUASHg;spec/connections/1.0/invitation",
    "@id": "1b62e664-a8d9-4c97-bb7a-2ba3b5329ebb",
    "recipientKeys": [
      "Gsc9q2FskuKYH2bAMnd3UkQadEkJ4QFwwA8RUdyGqsTo"
    ],
    "label": "faber.agent",
    "serviceEndpoint": "https://0639b9bd3d2a.ngrok.io"
  },
  "invitation_url": "https://0639b9bd3d2a.ngrok.io?c_i=eyJAdHlwZSI6ICJkaWQ6c292OkJ6Q2JzTlloTXJqSGlxWkRUVUFTSGc7c3BlYy9jb25uZWN0aW9ucy8xLjAvaW52aXRhdGlvbiIsICJAaWQiOiAiMWI2MmU2NjQtYThkOS00Yzk3LWJiN2EtMmJhM2I1MzI5ZWJiIiwgInJlY2lwaWVudEtleXMiOiBbIkdzYzlxMkZza3VLWUgyYkFNbmQzVWtRYWRFa0o0UUZ3d0E4UlVkeUdxc1RvIl0sICJsYWJlbCI6ICJmYWJlci5hZ2VudCIsICJzZXJ2aWNlRW5kcG9pbnQiOiAiaHR0cHM6Ly8wNjM5YjliZDNkMmEubmdyb2suaW8ifQ=="
}`

- Filter connections

> Request
`curl -X GET "http://localhost:8021/connections?tags=tag1" -H "accept: application/json"`

> Response
`{
  "results": [
    {
      "updated_at": "2021-05-20 12:06:41.865730Z",
      "created_at": "2021-05-20 12:06:41.865730Z",
      "accept": "manual",
      "rfc23_state": "invitation-sent",
      "their_role": "invitee",
      "routing_state": "none",
      "state": "invitation",
      "invitation_mode": "once",
      "connection_id": "8e1d9605-5843-4844-99d1-96141329e006",
      "invitation_key": "Gsc9q2FskuKYH2bAMnd3UkQadEkJ4QFwwA8RUdyGqsTo",
      "metadata": {
        "tags": [
          "tag1",
          "tag3"
        ]
      }
    }
  ]
}`

Based on @burdettadam idea, https://github.com/sicpa-dlab/aries-cloudagent-python/issues/49.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 12:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    Issue cred store cred done
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 19:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    Align with rfcs for error states in issue cred and present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RFCs 36, 37, 453 state that exchange states go to null on both sides on error; 454 uses "abandoned".

This work sets states accordingly where possible (unless there is no such record or the problem is storage itself), but does not (yet) send problem reports - that's another PR for the near-ish future.

In issue-credential, separate store-credential from send-ack: whether storage succeeds or fails, the protocol owes an ack because acknowledgement is to credential receipt, not storage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 13:52:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    DIDX create-request [return ConnRecord]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work left from #1174 and #1137.

- /didexchange/create-request now return ConnRecord
- Based upon feedback from @domwoe and  @andrewwhitehead, this will make it more consistent
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 00:24:56 +0000 UTC
    </div>
</div>


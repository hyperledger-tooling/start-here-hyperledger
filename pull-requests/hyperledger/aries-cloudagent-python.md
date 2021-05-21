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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1180" class=".btn">#1180</a>
            </td>
            <td>
                <b>
                    fix: use injected document loader for pyld calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 08:34:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1179" class=".btn">#1179</a>
            </td>
            <td>
                <b>
                    Add `resolve_with_metadata` method to DID resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This metadata includes information on how the DID was resolved, enabling the caller to make decisions about whether it accepts DID Documents resolved remotely or from a particular resolver, etc.

Props to @Luis-GA for doing most of the legwork on this feature.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 17:37:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1178" class=".btn">#1178</a>
            </td>
            <td>
                <b>
                    fix: don't load indy resolver if no indy ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 15:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Make BaseResolver.supports async and prefer regex matching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR extends the `BaseResolver.supports` method to be asynchronous and to take a `Profile` to support such use cases as retrieving resolver connections from storage and checking DIDs supported by those resolver connections. Additionally, this PR adds `supported_did_regex` as a value intended to be implemented by subclasses of `BaseResolver` and used in the default `supports` implementation. This changes the previous behavior of matching on the DID method alone to regex matching, granting more flexibility in how resolvers are selected to handle DID resolution.

`supported_methods` remains functional to prevent breaking resolver plugins already in the wild but is marked as deprecated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 03:48:53 +0000 UTC
    </div>
</div>


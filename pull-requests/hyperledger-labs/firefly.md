---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/171" class=".btn">#171</a>
            </td>
            <td>
                <b>
                    Firefly chaincode for Fabric integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This provides the counterpart of the Ethereum Solidity contract that performs the `pinBatch` function

The event contains the following properties:
```
  {
    "chaincodeId": "firefly",
    "blockNumber": 91,
    "transactionId": "ce79343000e851a0c742f63a733ce19a5f8b9ce1c719b6cecd14f01bcf81fff2",
    "eventName": "BatchPin",
    "payload": "eyJzaWduZXIiOiJ1MHZnd3U5czAwLXg1MDk6OkNOPXVzZXIyLE9VPWNsaWVudDo6Q049ZmFicmljLWNhLXNlcnZlciIsInRpbWVzdGFtcCI6eyJzZWNvbmRzIjoxNjMwMDA1OTcyLCJuYW5vcyI6MTU2ODY4MDAwfSwibmFtZXNwYWNlIjoibmFtZXNwYWNlIiwidXVpZHMiOiJ1dWlkcyIsImJhdGNoaGFzaCI6ImJhdGNoSGFzaCIsInBheWxvYWRSZWYiOiJwYXlsb2FkUmVmIiwiY29udGV4dHMiOlsiY29udGV4dDEiLCJjb250ZXh0MiIsImNvbnRleHQzIl19",
    "subId": "sb-0910f6a8-7bd6-4ced-453e-2db68149ce8e"
  }
```

`payload` is a byte array of a JSON structure:
```
{
  "signer": "u0vgwu9s00-x509::CN=user2,OU=client::CN=fabric-ca-server",
  "timestamp": {"seconds":1630005972,"nanos":156868000},
  "namespace": "namespace",
  "uuids": "uuids",
  "batchhash": "batchHash",
  "payloadRef": "payloadRef",
  "contexts": ["context1", "context2", "context3"]
}
```

The timestamp is of type `github.com/golang/protobuf/ptypes/timestamp`, which contains the nano second units as necessary for a Raft consensus where block intervals are at the millisecond level
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 20:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/170" class=".btn">#170</a>
            </td>
            <td>
                <b>
                    Replace "ID" with "Id" in JSON response fields
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
        Created At 2021-08-25 17:03:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    Alter datatype routes to query by name rather than ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Old route is now deprecated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 15:19:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Add maintainers as CODEOWNERS for /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the issue of requiring Nick's approval for anything that touches `/docs`. The intention was that he _could_ approve anything that _only_ modified `/docs`, but the way `CODEOWNERS` works, only the last rule to match gets applied, which meant global owners couldn't approve anything in `/docs`. I think this is the simplest solution to achieve what we want.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 12:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    Handle token_pool_rejected, add new transaction type for token pools
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
        Created At 2021-08-24 21:30:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    Add GET routes for token pools
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
        Created At 2021-08-24 19:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Rename token fields to match backend changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Counterpart to the field renames in https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/15. E2E tests are expected to fail until that PR is merged and released as a Docker image.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 16:00:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Create a batchpin utility for common utility between broadcast/private
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #159 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 16:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    Reject token pool events with duplicate info
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
        Created At 2021-08-23 16:22:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/162" class=".btn">#162</a>
            </td>
            <td>
                <b>
                    Add "confirm" parameter when creating token pools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR primarily adds the "confirm" parameter to token pool creation, which routes a request from Asset Manager to the Sync Async Bridge.

I also realized that by using the approach here (passing in a `RequestSender` callback), the circular dependency between `syncasync` and `syshandler` could be broken. I adjusted the other 3 existing sync-async operations (confirmed broadcast, confirmed private, request reply) to follow the same pattern. This means that `syncasync` now contains no logic at all for _sending_, only logic for tracking inflight IDs and unpacking system events to match them up.

Open to feedback on whether this callback pattern is the optimal design, but I do think removal of the circular calls makes the code easier to trace.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 15:28:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    Add an "id" parameter to SendMessageWithID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Given the method naming, it feels more intuitive to pass this in (rather
than requiring the sender to set it on a nested field before invoking).

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 21:06:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    Make sync-async helpers less specific to messaging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changeset simplifies the `inflightRequest` interface and adds 3 new generic constructs:
* `inflightResponse`
* `requestType`
* `requestSender`

The core helpers of sync-async (`sendAndWait` and `eventCallback`) now deal with these generic types and perform much less messaging-specific inspection of the requests and responses. There are clearer extension points for new request-response flows that may or may not relate to messaging at all.

The end goal is that this will make it easier to wrap tokens (and other future operations) in sync-async handlers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 15:09:39 +0000 UTC
    </div>
</div>


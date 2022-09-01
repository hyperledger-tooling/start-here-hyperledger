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
                PR <a href="https://github.com/hyperledger/firefly/pull/1035" class=".btn">#1035</a>
            </td>
            <td>
                <b>
                    remove legacy namespace query for organizations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1032 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 17:15:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1034" class=".btn">#1034</a>
            </td>
            <td>
                <b>
                    Routes to directly publish blob/JSON data to shared storage (IFPS etc.)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A small extension to external API routes, that let you initiate uploads through your public storage plugin directly.

Unlike with the full on-chain/off-chain orchestration capabilities, no modification is made to the data, and no batching happens.

So this is the feature you would use for example to publish the metadata+binary of an NFT.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 17:05:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1033" class=".btn">#1033</a>
            </td>
            <td>
                <b>
                    Update manifest for v1.1.0-rc.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updates EthConnect, EVMConnect, and FireFly Signer
- Fixes the tests for EVMConnect:
   - They were actually running EthConnect (missing env var)
   - The archive logs weren't distinguished uniquely
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 21:50:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    update event docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                in a chain with #1028 

not currently published on my github pages due to hosting another doc changes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 20:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1028" class=".btn">#1028</a>
            </td>
            <td>
                <b>
                    Add status information for subscriptions & contract listeners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 If the `fetchstatus` query param is supplied when querying `subscriptions` or `listeners` by ID, firefly will return additional status information, if it is available.

### Contract listeners:
FF environments connected to evm connectors will return listener checkpoint formation under the `status` key.

Example query: `http://localhost:5000/api/v1/namespaces/default/contracts/listeners/92e3bc0c-3c3f-455b-81d3-4124a0270b1d?fetchstatus`

Response:
```
{
    "id": "92e3bc0c-3c3f-455b-81d3-4124a0270b1d",
    "interface": {
        "id": "30775d45-61af-4f76-9d35-69b5d8ffbf42"
    },
    "namespace": "default",
    "name": "0182f410-a686-79ed-23a5-ac8c62acbf51",
    "backendId": "0182f410-a686-79ed-23a5-ac8c62acbf51",
    "location": {
        "address": "0x62d365e68fc55845ba904acef688feba7a598c9c"
    },
    "created": "2022-08-31T13:21:48.1687995Z",
    "event": {
        "name": "Changed",
        "description": "",
        "params": [
            {
                "name": "from",
                "schema": {
                    "type": "string",
                    "details": {
                        "type": "address",
                        "internalType": "address",
                        "indexed": true
                    }
                }
            },
            {
                "name": "value",
                "schema": {
                    "type": "integer",
                    "details": {
                        "type": "uint256",
                        "internalType": "uint256"
                    }
                }
            }
        ]
    },
    "signature": "Changed(address,uint256)",
    "topic": "bsc",
    "options": {
        "firstEvent": "oldest"
    },
    "status": {
        "checkpoint": {
            "block": 0,
            "transactionIndex": -1,
            "logIndex": -1
        }
    }
}
```

### Subscriptions
Subscriptions will provide offset information if available

Example Query: `http://localhost:5000/api/v1/namespaces/default/subscriptions/32cddc74-cc1a-4493-b376-45781e2d8d35?fetchstatus`

Response:
```
{
    "id": "32cddc74-cc1a-4493-b376-45781e2d8d35",
    "namespace": "default",
    "name": "simple-storage",
    "transport": "websockets",
    "filter": {
        "message": {},
        "transaction": {},
        "blockchainevent": {}
    },
    "options": {
        "firstEvent": "-1",
        "withData": false
    },
    "created": "2022-08-31T17:13:04.295134Z",
    "updated": null,
    "status": {
        "currentOffset": 31
    }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 17:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1027" class=".btn">#1027</a>
            </td>
            <td>
                <b>
                    Use advisory lock instead of exclusive lock on events table
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Advisory locks are identified with a 64-bit integer, so I've put in place a
rudimentary mapping from namespace names to a (probably) unique int64.
This should ensure consistent ordering for the writes to the events table
within a particular namespace, without blocking reads or other namespaces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 17:39:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1026" class=".btn">#1026</a>
            </td>
            <td>
                <b>
                    Allow null signer on transfers to account for non-archive indexing of historical transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1023 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 13:21:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1022" class=".btn">#1022</a>
            </td>
            <td>
                <b>
                    [identity-tutorial] identity tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tutorial to guide user through creating a Custom Identity in FireFly.

References https://github.com/hyperledger/firefly/issues/621
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 19:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    Allow any plugin to terminate the system on a bad event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Terminating the system is better than leaving it up in a crippled state.

Closes #957
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 18:52:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1019" class=".btn">#1019</a>
            </td>
            <td>
                <b>
                    Clean up event manager unit tests
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
        Created At 2022-08-30 17:25:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1018" class=".btn">#1018</a>
            </td>
            <td>
                <b>
                    add another account for fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Anna Jackson <anna.jackson@kaleido.io>

Fixes #1011 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 09:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    adds `fetchreference` to /events/:id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When provided, firefly will include the record that the `ref` field references in the response body.

closes #1016 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 02:33:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1015" class=".btn">#1015</a>
            </td>
            <td>
                <b>
                    Add firefly-signer to manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 19:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1012" class=".btn">#1012</a>
            </td>
            <td>
                <b>
                    Namespaces reference section + moonbeam docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs are live here: https://shorsher.github.io/firefly/head/reference/namespaces.html


in a chain with #966 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 15:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1010" class=".btn">#1010</a>
            </td>
            <td>
                <b>
                    Update Good First Issue Link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 14:18:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1009" class=".btn">#1009</a>
            </td>
            <td>
                <b>
                    Ensure new namespaces are up during multi_tenancy test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1008
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 16:39:05 +0000 UTC
    </div>
</div>


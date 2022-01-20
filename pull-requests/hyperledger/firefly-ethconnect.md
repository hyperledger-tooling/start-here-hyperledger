---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Add query support to / POST payload (webhook)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the "webhook" post on `/` to accept a new message type of `Query` (in addition to existing `SendTransaction` and `DeployContract` payloads).

The `Query` payload:
- Extends `SendTransaction` accepting all the same fields
- Adds a `blockNumber` field that defaults to `latest` and supports the same strings as the existing query APIs

https://github.com/kaleido-io/firefly-ethconnect/blob/e726955992f768362e875388eacd0252d148cfc9/internal/messages/messages.go#L148-L152

Here's a super minimal example to call the `get` method of simple storage (noting I've trimmed down the method ABI to just what's needed - you could put the full JSON in there, with `inputs` and `stateMutability` etc. etc.):

```json
{
    "headers": {
        "type": "Query"
    },
    "to": "0x93A82a40d0297c126b0c6ee8334A8639233F8d39",
    "method":   {
        "name": "get",
        "outputs": [{
            "type": "uint256",
            "internalType": "uint256"
        }]
    },
    "params": []
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 04:55:17 +0000 UTC
    </div>
</div>


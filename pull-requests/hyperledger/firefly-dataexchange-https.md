---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-dataexchange-https/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Destination verifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Indik <gabriel.indik@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 01:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-dataexchange-https/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Add destinations improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When sending a message or transferring a blob, the recipient ID can now contain an additional identifier. Also, the sender can be explicitly included which may also contain an additional identifier.

Example:
`POST /api/v1/messages`

Payload:
```json
{
    "recipient": "org-b/ns-a",
    "sender": "org-a/ns-x",
    "message": "test 1-2-3"
}
```

Response:
```json
{
    "requestId": "cee8e73e-4a97-4be7-abc8-f82de1e62939"
}
```

Sender receives event:
```json
{
    "id": "58e7a4b8-046e-478b-a82c-daa9eb9aae01",
    "type": "message-delivered",
    "message": "test 1-2-3",
    "sender": "org-a/ns-y",
    "recipient": "org-b/ns-x",
    "requestId": "cee8e73e-4a97-4be7-abc8-f82de1e62939"
}
```

Recipient receives event:
```json
{
    "id": "8d3351a8-bb83-4ce2-906d-4d099f8e2492",
    "type": "message-received",
    "sender": "org-a/ns-y",
    "recipient": "org-b/ns-x",
    "message": "test 1-2-3"
}
```

Similarly when transferring blobs:
`POST /api/v1/transfers`

Payload:
```json
{
    "path": "/photo.jpg",
    "sender": "org-a/ns-x",
    "recipient": "org-b/ns-y"
}
```

Response:
```json
{
    "requestId": "ba830d2c-dd39-48ce-ab70-dbfa610dc606"
}
```

Sender receives event:
```json
{
    "id": "16354dfb-1644-404e-a23c-51dd62d0d5d9",
    "type": "blob-delivered",
    "path": "/photo.jpg",
    "sender": "org-a/ns-x",
    "recipient": "org-b/ns-y",
    "requestId": "ba830d2c-dd39-48ce-ab70-dbfa610dc606"
}
```

Recipient receives event:
```json
{
    "id": "bb745fe8-8837-436f-9d20-315dc0da01a5",
    "type": "blob-received",
    "sender": "org-a/ns-x",
    "recipient": "org-b/ns-y",
    "path": "received/org-a/ns-x/photo.jpg",
    "hash": "9707a075644e450ebec9c87dfa3b79b53e51f878cfc0394b80c30949f4d2000c",
    "size": 146866,
    "lastUpdate": 1658437514514
}
```

Notice the folder structure, the file is stored in a subdirectory based on the additional identifier.
Note also that these changes are backward compatible as the additional identifiers are optional.

Also included in this PR:
 - Updated certificates for development (original ones were expired)
 - Headers updated (2021 -> 2022)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 14:35:12 +0000 UTC
    </div>
</div>


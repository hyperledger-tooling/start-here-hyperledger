---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    Update platformroutes.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### What this PR does / why we need it:
`/api/peersStatus/:channel` endpoint does not work if `:channel` is channel name (e.g. mychannel) because `proxy.getPeersStatus()` expects `channel_genesis_hash` as parameter. I have changed the code to reflect such differences.

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
NONE
```release-note

```

#### Additional documentation, usage docs, etc.:

```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 17:14:53 +0000 UTC
    </div>
</div>


---
layout: default
title: firefly-cli
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Check HTTP status code for contract deploy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This also revealed that it's not necessary to separately call
RegisterContract if DeployContract was already called on the node with
registeredName (it returns 409 since the contract was already registered).

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 20:58:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Set _busy_timeout=5000 by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With SQLite default parameters, the following error is reasonably likely under load:
```
{"error":"FF10116: Database insert failed: database is locked"}
```

Setting a `_busy_timeout` on the SQLite URL by default should reduce the likelihood of this.
Lots more interesting information here: https://github.com/mattn/go-sqlite3/issues/274
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 01:23:10 +0000 UTC
    </div>
</div>


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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Do not remove images on ff reset/remove
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
        Created At 2021-07-19 17:00:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Add CODEOWNERS
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
        Created At 2021-07-15 15:24:50 +0000 UTC
    </div>
</div>


---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    SqlMerkleState Remove Index tables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the index tables and replaces the last use of them in list_leaves with a recursive query.  This has considerable performance improvement in Postgres, and minimal impact for Sqlite.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 15:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    Add feature deps for family-command-workload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the feature `"family-command-workload"` such that compiling like:

```
$ cargo check --manifest-path libtransact/Cargo.toml --features family-command-workload
```

will successfully compile.

It also makes the indenting consistent in the Cargo.toml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 14:00:58 +0000 UTC
    </div>
</div>


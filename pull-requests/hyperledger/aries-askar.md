---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    DB Connection Pooling and Proxying docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add some documentation explaining Database Proxying, referencing [pgBouncer](https://www.pgbouncer.org/) and [AWS RDS Proxy](https://aws.amazon.com/rds/proxy/).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 12:29:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Add DB benchmark
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a benchmark using [`criterion`](https://github.com/bheisler/criterion.rs) to benchmark DB performance,
specifically when the DB has a large number of profiles/items/items_tags.

Benchmark is heavily based on `tests/store_key.rs`

Please feel free to be extremely pedantic (`-Wclippy::pedantic -Wclippy::nursery`)

Related to #195 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 09:07:35 +0000 UTC
    </div>
</div>


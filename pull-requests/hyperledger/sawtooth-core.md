---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    fix clippy warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Joseph Livesey [joseph.livesey@btp.works](mailto:joseph.livesey@btp.works)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-22 21:00:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2439" class=".btn">#2439</a>
            </td>
            <td>
                <b>
                    change TransactionCommitCache to LRU
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TransactionCommitCache is currently based on a HashSet which depends on its clients to properly clean up their items in a timely fashion. However, under high load circumstances, this can be too long resulting in quiet OOM issues and in practice freezing the whole network.

This changes the TransactionCommitCache to an uluru LRU. This is safe since the commit cache is based on data that cannot change and the worst that happens on a miss is a refetch from the store.

uluru is also updated to 3.0.0 which requires a minor change to `block_validator.rs` to account for the changed construction
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-22 17:59:36 +0000 UTC
    </div>
</div>


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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    Add fly-id based idempotency for LevelDB (as implemented for MongoDB)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `fly-id` (/`kld-id`) query param for idempotent submission of transactions, using an external ID combined with `fly-acktype=receipt` (/`kld-acktype`), functions based on the DB requiring uniquness.

LevelDB doesn't have this as a first class construct, so we need to implement it at the ethconnect code layer.
 
Solving this e2e meant implementing an `overwrite` option through the stack, to pick between "keep trying to insert, with overwrite" functionality when storing the final reply, vs. "try inserting, and fail immediately" functionality when storing the initial `acktype=receipt`.

I also found an unrelated issue with the in-memory receipt store, where it was not retaining _any_ history by default when configured via YAML. A real pain for FireFly CLI based environments.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 00:38:14 +0000 UTC
    </div>
</div>


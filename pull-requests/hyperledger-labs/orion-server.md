---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    Perform mvcc read validation in parallel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span>
            </td>
            <td>
                The current implementation goes over each read operation- one by one- and validates if it was already written in this block and if the read version matches the current version.

The current design avoids redundant reading of keys' versions by checking first if previous pending operations overwrote this key. But this enforces a sequential implementation.

Instead, this PR takes an eager, optimistic approach.
We assume that conflicts are rare, so we eagerly read all keys' versions in parallel and check if the version matches.
Then, if all is OK, we continue to check the operations one by one to see if one operation invalidates another.

This removes the bottleneck caused by the expensive version read operation.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-29 13:48:14 +0000 UTC
    </div>
</div>


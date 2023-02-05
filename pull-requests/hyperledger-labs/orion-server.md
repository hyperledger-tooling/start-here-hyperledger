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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    Avoid instantiating the default marshaller before each use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix typo in class name

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 10:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Go 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">security</span>
            </td>
            <td>
                Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 08:22:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Allow issuing cert with URI instead of IP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                This is used by Orion's benchmark to issue certificates for the servers.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 13:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Use lock-free map for LevelDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span>
            </td>
            <td>
                - Replacing map with sync.Map
- Caching DB snapshot after commit to avoid creating a snapshot for each Get operation
- Modifying cache to return byte array to avoid code duplication
- Remove Db lock because levelDB is already protected
- Reduce code duplication in Open()

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 14:58:42 +0000 UTC
    </div>
</div>

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


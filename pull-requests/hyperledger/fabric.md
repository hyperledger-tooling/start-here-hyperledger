---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4208" class=".btn">#4208</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove ORDERER_TRANSACTION
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I97bdd9fbc60195bbaf7c4486e43dbf7f28bbff66

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

The ORDERER_TRANSACTION type is no longer used, reject it everywhere

#### Related issues

Issue: #3515 #4204
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 16:44:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4207" class=".btn">#4207</a>
            </td>
            <td>
                <b>
                    system channel cleanup - remove replicator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cleaned dependencies on system channel from the `orderer/common/cluster/replication.go`.

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

As described in issue #4202 .

#### Related issues

Issue: #4202 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 15:14:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4201" class=".btn">#4201</a>
            </td>
            <td>
                <b>
                    Restrict WAL usage to node.go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/fabric/issues/4199
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-06 23:30:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4196" class=".btn">#4196</a>
            </td>
            <td>
                <b>
                    system channel clean up - msgprocessor package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Cleaned dependencies on system channel from the msgprocessor package.
2. Removed templator usages.

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

As described in issue #4189.

#### Additional details

#### Related issues

Issue: #4189.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 14:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4195" class=".btn">#4195</a>
            </td>
            <td>
                <b>
                    Remove requests from BFT memory pool when syncing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a BFT node commits a block, it goes through the transactions in the block and searches whether they exist in the in-memory pool, and if so, it removes them from the pool.

When a follower node syncs blocks from another node, the requests of these blocks still remain in its request pool. They not only take up memory, but also holds the semaphore resources which throttle needlessly the client.

This commit goes through the requests of a block that is committed through synchronization and removes them as well. This is needed because the library only sees the last block committed during synchronization and not the entire range.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 08:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4193" class=".btn">#4193</a>
            </td>
            <td>
                <b>
                    Update SmartBFT library to latest version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 10:52:00 +0000 UTC
    </div>
</div>


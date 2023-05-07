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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4192" class=".btn">#4192</a>
            </td>
            <td>
                <b>
                    Release commit for v2.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add docs and release notes for v2.5.1 release.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 02:44:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4191" class=".btn">#4191</a>
            </td>
            <td>
                <b>
                    cleanup of the onboarding package + removed initializeEtcdraftConsenter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Cleaned dependencies on the onboarding package, so the package could be deleted.
2. Removed initializeEtcdraftConsenter

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

As described in issue #4184.

#### Additional details

#### Related issues

Issue: #4184.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-30 16:48:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4190" class=".btn">#4190</a>
            </td>
            <td>
                <b>
                    Ordere v3: remove sys chan: clean consensus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I600362026a64d792782b3bf9d4037348821a4a4e

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Ordere v3: remove sys chan: clean consensus, remove InactiveChainRegistry from consenter
Remove inactive.Chain

#### Related issues

Issue: #4185 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-30 09:41:42 +0000 UTC
    </div>
</div>


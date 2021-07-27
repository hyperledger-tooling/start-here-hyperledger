---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Add MAINTAINERS.md, CONTRIBUTING.md and other required files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a proposed process for adding new maintainers, as well as a short guide on making contributions. I've also included several other required files to get us up to spec with: https://github.com/hyperledger-labs/hyperledger-community-management-tools/tree/main/repo_structure

Still missing is a CHANGELOG.md. I'm looking into ways to automate this. This PR will remain in draft state until existing maintainers have had time to discuss and agree on the process for adding new maintainers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 19:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Repeated groupinit messages: Make sure we sort the group members, before existence check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a case where we saw repeated `groupinit` messages being sent every time an unpinned message exchange was being performed in a request/reply scenario between two parties in the network.

The problem was the "_does the group already exist?_" check was being done using DB query with a hash calculated on an _unsorted_ list of members. Whereas the creation was correctly using `group.Seal()` which sorts the list of members before hashing. So we would repeat the creation over and over.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 14:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Avoid writing pins that can never be resolved
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We saw a situation where broadcasts were not being processed by a network, and the reason logged was:
```
[2021-07-21T13:29:22.474Z] DEBUG Message 29ef8ae6-06a0-461c-b9d1-fa754e6f3315 pinned at sequence 11775 blocked by earlier context f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d at sequence 10667 dbtx=oWj1wBCU pid=1 role=aggregator
```

This was in a FireFly environment where it had been rebuilt, with fresh FireFly databases, but using the same on-chain contract. The context of the batches that could not be processed were organizataion definitions.

Inspecting the `pins` database table, we could see a list of un-dispatched pins for the same context (e.g. the same on-chain organization ID):
```
  seq  | masked |                               hash                               |               batch_id               | idx | dispatched |       created       
-------+--------+------------------------------------------------------------------+--------------------------------------+-----+------------+---------------------
     7 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 43b86d42-63de-40af-aa5b-389577cbff0a |   0 | f          | 1626873947548837682
    10 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 9f4f148d-0e9b-4cc9-80f1-1eb2dd7d7549 |   0 | f          | 1626873947701026182
    11 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 16c95a7b-5459-4d33-93b5-4e9ffb7a037f |   0 | f          | 1626873947813108703
    17 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 041ef318-713d-49f1-9837-6a0c8f7a7d03 |   0 | f          | 1626873948148579427
    18 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | adb54417-ab2f-4545-88d4-3bdaa85902a8 |   0 | f          | 1626873979795296873
    30 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | d8fec3c5-98d3-4fb6-96b8-5008471b5a06 |   0 | f          | 1626873980089044029
    31 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | d8fec3c5-98d3-4fb6-96b8-5008471b5a06 |   1 | f          | 1626873980092709323
  1275 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | b2e5cf70-748c-43db-bf53-8ffd2617be6c |   0 | f          | 1626873997040283520
  1276 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | d29e6e92-1897-4c98-af44-3a93143e754a |   0 | f          | 1626873997091277560
 10666 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 4de72a48-abff-46e7-bf6c-86b4bcbe45f0 |   0 | f          | 1626874141923359231
 10667 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 7a442e04-5c81-4d7f-a562-4b76c81ff106 |   0 | f          | 1626874141990760266
 11775 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 8fc90cde-1a2d-4d11-895f-cae1ee828a12 |   0 | f          | 1626874162367960540
 11776 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | ef5a83f8-b99a-4ee3-a98d-4390a8dd4db4 |   0 | f          | 1626874162428103422
```

The batch was **not** stored in the `batches` table, but looking in the `transactions` table where `ref` is the batch, we could see that the blockchain transaction had a `payloadRef` to IPFS that could be resolved.

From this we could work out that the problem is the batches were rejected **without being stored** ~surmising this is because the authors were not known, because they were from a previous chain where the organizations got defined in a different order to the current FireFly environment.~ - after further code inspection we do not verify the organization exists at this point. Rather just that the author identity can be resolved. However, the fact the batch is missing, but the pin is there was conclusive in the investigation.

The problem here is that we knew at the point we inserted the pin, it could never be resolved!!! ... so we shouldn't have inserted the pin at all. We should only have un-dispatched pins for cases where we are _waiting_ for data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 22:18:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Set max connections to 1 for SQLite and allow config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per https://github.com/hyperledger-labs/firefly-cli/pull/64 we've seen issues with SQLite returning:
```
FF10116: Database insert failed: database is locked
```

We're setting a default `_busy_timeout` in the CLI now, but it still seems the concurrency inherent in FireFly means it's easy to drive SQLite to a point it returns errors.
So the other approach is to limit the concurrent connections - and with 1 as the default that should not stress SQLite. Clearly that has a performance impact, but SQLite is primarily for lighter weight Dev scenarios where reliability matters more than performance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 14:35:41 +0000 UTC
    </div>
</div>


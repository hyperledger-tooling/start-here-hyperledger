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
                PR <a href="https://github.com/hyperledger/fabric/pull/4303" class=".btn">#4303</a>
            </td>
            <td>
                <b>
                    Ledger block cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit introduces an in-memory cache for the block storage of the ledger. It caches new blocks that are committed and assumes blocks are committed in-order and with consecutive sequences.

The block iterators now attempt to retrieve the blocks from the cache if possible before going to the block storage.

The intent is twofold:

1) Speedup the block Deliver API by not doing disk I/O when clients (peers, orderers) fetch blocks. 

2) Reduce the impact of the deliver API on the performance of writing new blocks into the ledger.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 19:27:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4301" class=".btn">#4301</a>
            </td>
            <td>
                <b>
                    remove kafka from documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

update documentation regarding the removal of Kafka

#### Related issues

issue #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 15:05:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4299" class=".btn">#4299</a>
            </td>
            <td>
                <b>
                    Create CITATION.cff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Please create a CITATION.cff file so researchers can cite this repo. Thank you.

#### Additional details


#### Related issues






            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 14:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4298" class=".btn">#4298</a>
            </td>
            <td>
                <b>
                    update Fabric to include fabric-config latest commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- dependency update


#### Description

update fabric-config version to include the latest commit

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:08:22 +0000 UTC
    </div>
</div>


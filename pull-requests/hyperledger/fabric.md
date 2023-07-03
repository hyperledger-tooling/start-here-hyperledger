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
                PR <a href="https://github.com/hyperledger/fabric/pull/4307" class=".btn">#4307</a>
            </td>
            <td>
                <b>
                    [Fix]: Provide a meaningful error for cert sanitization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit handles the error where the certificate sanitization procedure fails to construct the certificate chain due to misconfiguration. Before this commit, the peer will simply fail with panic without a clear explanation of what exactly was wrong.

Addresses (#4302).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 11:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4305" class=".btn">#4305</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: censorship monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- New feature

#### Description

BFT Block Puller: censorship monitor

- BFT header receivers that pull headers from the orderers, and keep the time and number of the last one.
- A BFT censorship monitor which compares the progress of headers relative to blocks, and triggers an alert if a header is ahead of the block stream for more than a certain time.

#### Related issues
#4306 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 08:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4304" class=".btn">#4304</a>
            </td>
            <td>
                <b>
                    Add SmartBFT consensus knobs to configtx.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The configtx.yaml now has the SmartBFT consensus knobs as in the Fabric samples

#### Related issues

https://github.com/hyperledger/fabric/issues/4295

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 08:03:54 +0000 UTC
    </div>
</div>

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


---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4406" class=".btn">#4406</a>
            </td>
            <td>
                <b>
                    Add Rpc method name when logging IOException
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add Rpc method name when logging IOException

## Fixed Issue(s)
fixes #4405 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 05:51:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4395" class=".btn">#4395</a>
            </td>
            <td>
                <b>
                    logs JSON-RPC request and responses in TRACE mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pedro Novais <jpvnovais@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Allows logging JSON-RPC requests and responses. Very convenient when debugging clients/applications.

Logging example
```
2022-09-14 17:25:07.147+01:00 | vert.x-worker-thread-19 | TRACE | JsonRpcExecutorHandler | [{"id":2,"jsonrpc":"2.0","method":"eth_blockNumber","params":[]},{"id":2,"jsonrpc":"2.0","method":"eth_getBlockByNumber","params":["latest",false]}]
2022-09-14 17:25:07.159+01:00 | vert.x-worker-thread-19 | TRACE | JsonRpcExecutorHandler | [{"jsonrpc":"2.0","id":2,"result":"0x1"},{"jsonrpc":"2.0","id":2,"result":{"number":"0x1","hash":"0xd5e013779272ec9c7494e89cb62a9f777d1efdf4086ce58390f31c1629ec72ec","mixHash":"0xb02df79657ae2c9b7a86e477f8a951679d70a524eae627e1bacbcf2083c422fe","parentHash":"0xb576a24aceaa5585645d9f83acddc99c470e0a6ee0064670679aff42db3afd9d","nonce":"0x0000000000000000","sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347","logsBloom":"0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000","transactionsRoot":"0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421","stateRoot":"0x166ed98eea93ab2b6f6b1a425526994adc2d675bf9a0d77d600ed1e02d8f77df","receiptsRoot":"0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421","miner":"0x0000000000000000000000000000000000000000","difficulty":"0x0","totalDifficulty":"0x1","extraData":"0x","baseFeePerGas":"0x342770c0","size":"0x201","gasLimit":"0xa00400","gasUsed":"0x0","timestamp":"0x6297609a","uncles":[],"transactions":[]}}]
```
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 16:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4392" class=".btn">#4392</a>
            </td>
            <td>
                <b>
                    [MINOR] add BftExtraData toString
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

To fix https://github.com/hyperledger/besu/security/code-scanning/654

In most cases, calling the default implementation of toString in java.lang.Object is not what is intended when a string representation of an object is required. The output of the default toString method consists of the class name of the object as well as the object's hashcode, which is usually not what was intended.


## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 02:21:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4391" class=".btn">#4391</a>
            </td>
            <td>
                <b>
                    Logging: peer table refresh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                Improve UX of log messages related to peer table refresh and neighbours

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 02:18:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4390" class=".btn">#4390</a>
            </td>
            <td>
                <b>
                    Bugfix concurrent legacy transaction eviction in BaseFee txpool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Address a concurrency problem with transaction eviction, where we try to evict a transaction that has been concurrently removed from the dynamic transaction pool set.
* make the static transaction pool comparator (base-fee-only transactions) safe for non-1559 transactions, in case we attempt to remove a non-1559 transaction.
* check to see if removed transaction has a basefee before attempting to remove it from the static (base-fee only) transaction set.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4343


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 21:11:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4388" class=".btn">#4388</a>
            </td>
            <td>
                <b>
                    RLP zero encoding fix.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Updates the RLPOutput encoding to encode 0 as 0x80

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4284 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 12:27:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4387" class=".btn">#4387</a>
            </td>
            <td>
                <b>
                    Revise Memory Expansion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Move from a perfect fit memory expansion model to an exponential expansion model.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 08:24:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4386" class=".btn">#4386</a>
            </td>
            <td>
                <b>
                    Replace boolean return with BlockImportResult object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
BlockImporter currently returns a `boolean true` when: 

- A  block is successfully imported or 
- the block is already in the blockchain

If the same block is mistakenly tried to be imported more than once, `PersistBlockTask` will log "Imported #" for each try, ignoring that the block is actually imported only once, resulting in misleading logging. 

This PR changes the return type of `BlockImporter.importBlock` to return an object `BlockImportResult` instead of `boolean`.

`BlockImportResult` implements `isImported`, which has the current behaviour of the importBlock: returns `true` if the block is successfully processed or is already in the chain. In addition, it contains a getStatus that, if needed, can be used to distinguish whether the block was processed or was already in the chain. 

PersistBlockTask will look at the getStatus in order to decide what needs to be logged in the cleanup.  

## Fixed Issue(s)
fixes #4350

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 03:46:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4381" class=".btn">#4381</a>
            </td>
            <td>
                <b>
                    Snapsync persist state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">snapsync</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR avoids starting the download of the world state from scratch when restarting Besu

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 15:06:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4378" class=".btn">#4378</a>
            </td>
            <td>
                <b>
                    Quieten merkletrie exceptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Quieten the noisy non-critical MerkleTrieExceptions thrown during block production and transaction validation

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 19:36:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4377" class=".btn">#4377</a>
            </td>
            <td>
                <b>
                    WIP (feedback needed): Fix banning because of late response in eth/66
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

- The RequestManager commit that lessens the penalty should be somewhat straightforward. A late response is typically already punished with a timeout before (too many of which and we disconnect). Instead of immediately considering a late response a breach of protocol, we just consider it useless (again, too many of which and we disconnect).

- The not banning of maintained/static peers was a bit more difficult. I'm not sure if this is the right^TM way to do it, but a Peer object has no notion of it being static/maintained. And static nodes are also not instantiated in a single call, they are combined with bootnodes. So adding a `isStatic` field to EthPeer also seemed more trouble than it was worth. Therefore I settled on this solution, but there might be a better/simpler/more elegant one.

Feedback more than welcome!

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4320
Related to #4294

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

## TODO before merging
- [ ] Elaborate RequestManager commit message
- [ ] Elaborate in PeerDenylistManager commit message
- [ ] Fix test cases PeerDenylistManager 
- [ ] Add test case (with maintained/static peer) for PeerDenylistManager 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 15:41:10 +0000 UTC
    </div>
</div>


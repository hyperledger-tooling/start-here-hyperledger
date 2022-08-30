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
                PR <a href="https://github.com/hyperledger/besu/pull/4325" class=".btn">#4325</a>
            </td>
            <td>
                <b>
                    refactors to rely on blocks added, and behave like singleton
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Will not show ready for merge on startup when local stored chain is past ttd.
Uses block observer to determine state change

Signed-off-by: Justin Florentine <justin+github@florentine.us>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 17:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4318" class=".btn">#4318</a>
            </td>
            <td>
                <b>
                    Disable RocksDB Write Ahead Log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Disable RocksDB Write Ahead Log, this may create some issues to recover from a crash, but still need to test and try to find a compromise : Performance vs effort to recover from a crash 

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
        Created At 2022-08-26 16:02:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4316" class=".btn">#4316</a>
            </td>
            <td>
                <b>
                    ContainerTests - use tessera 22.1.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Use 22.1.7 docker image for Tessera. 
Not a required update, dependency change only.
https://github.com/ConsenSys/tessera/releases/tag/tessera-22.1.7

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 06:04:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4312" class=".btn">#4312</a>
            </td>
            <td>
                <b>
                    fix trie by asking peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

we may have an inconsistency in the worldstate trie. If this happens even if the cases are very rare and complex to reproduce this PR can help resolve the issue. Indeed if we detect a problem in the trie we can fix it directly by asking our peers for the correct version of the node 

We start by asking with the GetNodeData request (which will soon be deprecated but which is still compatible and more practical) and if the response is empty we try with GetTrieNode

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
        Created At 2022-08-25 12:04:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4311" class=".btn">#4311</a>
            </td>
            <td>
                <b>
                    Reducing verbosity during BWS errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Stacktrace can be retrieved by increasing the log level

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

## Fixed Issue(s)
fixes #4263

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 11:37:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4310" class=".btn">#4310</a>
            </td>
            <td>
                <b>
                    Log imported block info post merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                After the switch to PoS, info of the imported blocks are not more logged, this PR re-add the log when a block is imported via the NewPayload engine RPC call, and also update the info logged to remove ommers and add base fee.

Sample of the message:
`Imported #12,862,033 / 5 tx / 439,018 (1.5%) gas / base fee 7 wei / (0xb1b6d51e6382a1c88b42344f53d5321ee63bec0226fae502876af55e7109f431) in 0.028s.`

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

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
        Created At 2022-08-25 10:29:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4309" class=".btn">#4309</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] moved 4279 to 22.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">22.7.2</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

moved #4279 to 22.7.2

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 02:07:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4308" class=".btn">#4308</a>
            </td>
            <td>
                <b>
                    small variable renaming in AbstractJsonRpcTest
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
Some renaming that came to mind only after the merging  of #4286

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
        Created At 2022-08-24 15:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4306" class=".btn">#4306</a>
            </td>
            <td>
                <b>
                    update docker version on quorum ats executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

* Update docker version on executor used for acceptanceTestQuorum CI step (part of nightly CI pipeline)
* Also temporarily make acceptanceTestsQuorum run on this PR to see if it runs ok
* remove acceptanceTestsQuorum from PR build

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 05:32:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4305" class=".btn">#4305</a>
            </td>
            <td>
                <b>
                    update Tessera version and ubuntu for xl-machine-executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">22.7.2</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

* Update tessera docker image version to 22.1.6
* Update ubuntu version on xl machine executor in Circle CI config - this update is required for the tessera 22.1.6 docker image to run

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 04:08:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4304" class=".btn">#4304</a>
            </td>
            <td>
                <b>
                    Log the number of connected peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The number of connected peers is what matters. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 01:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4303" class=".btn">#4303</a>
            </td>
            <td>
                <b>
                    Reinstate Tessera tests with a fixed version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Use a fixed version of Tessera docker image. 
* Enable the ignored privacy tests that use Tessera 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 20:46:47 +0000 UTC
    </div>
</div>


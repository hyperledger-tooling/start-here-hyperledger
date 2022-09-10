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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4373" class=".btn">#4373</a>
            </td>
            <td>
                <b>
                    bugfix: BlockValidator should pass shouldPersist flag when getting worldstate
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
The 'remember block' and 'prepare payload' functions in MergeCoordinator uses a mutable worldstate to validate and process blocks, and should not mutate the current head worldstate during these operations.  This PR fixes a bug where we did not plumb the shouldPersist parameter through into the block validator.

The net result is that a preparePayload call could mutate the worldstate concurrenctly / incorrectly.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4372

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 21:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4370" class=".btn">#4370</a>
            </td>
            <td>
                <b>
                    Feature/prep 22.7.3
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
prep for 22.7.3 release

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
        Created At 2022-09-08 19:54:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4366" class=".btn">#4366</a>
            </td>
            <td>
                <b>
                    Update spotless config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Update the greclipse version in spotless as directed by build errors to reduce random formatting errors.

Also, update formatting to new version

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 14:19:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4364" class=".btn">#4364</a>
            </td>
            <td>
                <b>
                    Always return a transaction type for pending transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

This PR ensures that a pending transaction with transaction type 0 always returns its type when being serializes to JSON.

## Fixed Issue(s)
fixes #4248

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 12:46:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4362" class=".btn">#4362</a>
            </td>
            <td>
                <b>
                    prep for 22.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
prepare for 22.7.3 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 23:27:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4361" class=".btn">#4361</a>
            </td>
            <td>
                <b>
                    release versioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
release version for 22.7.2
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
        Created At 2022-09-07 22:17:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4359" class=".btn">#4359</a>
            </td>
            <td>
                <b>
                    Cherry pick release 22.7.2
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
Cherry picks for 22.7.2, on top of post-22.7.1 release snapshot commit:
```
PR      commit     Description
4351    20fc1b7f2    snapsync logging tweaks
4312    c57dcd99d    Fix trie node from peers
4325    101f5efbd    Pandas
4352    93109ecc2    Returns INVALID on timeout exception
4353    d20f0a8f4    Miner shutdown
4337    296025865    quieten rlp decode error logging
4347    6e8a906df    snapsync logging for clearer sync status
4336    8ee253982    Future tx nonce limits by sender
4327    f3fd946ed    Txpool eviction by tail
4335    2e08c5c09    Better CORS errors
4334    86c308096    RLP Decoding should not log at ERROR
4311    b25779149    BWS logging fix
4310    c321a85ef    Post-Merge logging for block info
4271    af65c86e6    Retry mechanism in import
4269    b3b8e0aae    Peer filter for disconnected peers
4237    dcb951eb7    JEMalloc Logging changes
4283    e5e6a679d    interpret an empty string (0x80) as an unsigned byte of 0
4268    113bd54c6    logging for breach of protocol
4298    a44cb1cab    reduce post-merge fast sync min peers
4299    16922cac8    reduce logging
```

edit: added Tessera and test container commits in order to pass CI:
```
4297     98e214ced   ignore the tests that use tessera enclave via docker
```

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
        Created At 2022-09-07 20:16:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4357" class=".btn">#4357</a>
            </td>
            <td>
                <b>
                    Avoid a cyclic reference while printing EngineExchangeTransitionConfigurationParameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

EngineExchangeTransitionConfigurationParameter is printed if logging is set to `TRACE`. In the current version it throws an exception while trying to print it, because of a circular reference. This PR avoids this circular reference and EngineExchangeTransitionConfigurationParameter is printed as expected.


## Fixed Issue(s)
fixes #4354

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 14:05:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4355" class=".btn">#4355</a>
            </td>
            <td>
                <b>
                    Log index is counted per block, not per transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

The log index returned by `eth_getLogs` is currently counted on a transaction basis, which is incorrect. The correct way is to have it unique per block. This PR changes it to the correct behavior.

## Fixed Issue(s)
fixes #4114

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 13:09:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4353" class=".btn">#4353</a>
            </td>
            <td>
                <b>
                    Always shutdown the mining executor on exit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

There is an issue that prevents the PoWMiner to stop cleanly, with the effect of taking 30 seconds before the timeout expires and Besu can stop.

Basically the miner executor was only shutdown when running, but not when it was idle, this PR always shutdown the executor when the mining is stopped


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4313

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 10:39:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4352" class=".btn">#4352</a>
            </td>
            <td>
                <b>
                    adds means to report causing exception up to RPC layer 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                so it can decide how to present it to the CL

fixes #4349 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 22:06:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4351" class=".btn">#4351</a>
            </td>
            <td>
                <b>
                    Wording tweaks for edge cases in PR #4347
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">22.7.2</span>
            </td>
            <td>
                Signed-off-by: Matt Nelson <matt.nelson@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
Changes previous fix (#4347) for #4346 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-06 15:40:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4347" class=".btn">#4347</a>
            </td>
            <td>
                <b>
                    Update snapsync logging for clearer sync status. Issue 4346.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span><span class="chip">22.7.2</span>
            </td>
            <td>
                Signed-off-by: Matt Nelson <matt.nelson@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
Fixes #4346.

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 16:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4345" class=".btn">#4345</a>
            </td>
            <td>
                <b>
                    waiting blockchain before stopping snapsync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR modifies the snapsync so that the heal is done throughout the download of the blocks. As long as we haven't downloaded all the blocks we change the pivot block to get closer to the head. this reduces the number of blocks to full sync

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
        Created At 2022-09-05 09:40:25 +0000 UTC
    </div>
</div>


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
                PR <a href="https://github.com/hyperledger/besu/pull/6045" class=".btn">#6045</a>
            </td>
            <td>
                <b>
                    Fixed eth_call before london fork for the calls without strict parameter
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
Fixed eth_call before London fork for the calls without `strict` parameters.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fix #5943
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 17:31:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6044" class=".btn">#6044</a>
            </td>
            <td>
                <b>
                    Time limited block creation
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 17:04:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6040" class=".btn">#6040</a>
            </td>
            <td>
                <b>
                    Fix 23.10.0 Breaking Changes changelog entry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes a wrong breaking change entry reported here #6031

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 07:59:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6038" class=".btn">#6038</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] fix links to issue 5772
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes link refs #6031 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 01:50:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6037" class=".btn">#6037</a>
            </td>
            <td>
                <b>
                    Fcu v2 defer fork validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                re-orders the validity checking and priority on forkchoice updated calls.

- payloadAttributes needs to be validated apart from new head validity, so there are now two steps for checking so that we can fail differently if the head being built on is missing or irrelevant to the building payload.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 14:14:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6036" class=".btn">#6036</a>
            </td>
            <td>
                <b>
                    Fix typos
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
        Created At 2023-10-16 11:54:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6035" class=".btn">#6035</a>
            </td>
            <td>
                <b>
                    Minor optimization on Eth_feeHistory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR has a minor optimization on Eth_feeHistory, on top of [this other optimization on Eth_feeHistory ](https://github.com/hyperledger/besu/pull/6011).

Instead of sorting rewardPercentiles for each block header, this PR sorts only once and the sorted list is used as a parameter for each call to compute rewards.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 11:45:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6034" class=".btn">#6034</a>
            </td>
            <td>
                <b>
                    fix incorrect argument passing in blockParameter of TraceCallMany class
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
fix incorrect argument passing code in blockParameter function of TraceCallMany class. only need to change one line of code

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixed #6033 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 04:53:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6029" class=".btn">#6029</a>
            </td>
            <td>
                <b>
                    docs: fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                thx to @vuittont60
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 04:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6028" class=".btn">#6028</a>
            </td>
            <td>
                <b>
                    remove code duplication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Noticed that these lines of code were duplicated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 00:18:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6027" class=".btn">#6027</a>
            </td>
            <td>
                <b>
                    Mining options refactor
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

Before adding new mining options for upcoming features, I took some time to review and refactor mining options.
Mining parameters are a bit odd when compared to other options, since they do not follow the same pattern of using immutables, as for txpool options, stable options are defined in `BesuCommand`, and since that file is already too big, adding more options there should be avoided. 

For the refactoring I have reapplied most of the solutions used for the refactoring of txpool options (see #5772 if interested), with some novelty, since for mining configuration a new feature is required, that is having the possibility to update the value of some options at runtime.
One notable difference with #5772, is that _stable_ and _unstable_ options are no more split on two classes, since it make more sense to keep all the related options in a single place, also because some validations could make use of a mix of stable and unstable options, and for that it is better to have all of them in a single place.

To implement the _update at runtime_ feature, in a thread safe way, unfortunately it is not possible to use the immutables library directly, so instead of using annotations, some code has to be added to the `MiningParameters` class to manage the updatables options. If the proposed solution prove to be effective and looks good, after it stabilize, we can also think of extending the immutables library to support this, or introduce our own annotations, or find another library that is best suited for managing configuration.
The _updatable_ parameters work like that: 
- on startup their initial value is set, as usual from config file or CLI, 
- these parameters have also a _set_, along with the normal _get_ one, 
- the values are kept in _volatile_ fields, to make it multi thread friendly
- Note that initial values are kept in case it is needed, even if the parameters  then updated at runtime, 

The proposed implementation also has the goal to centralize all the parameters in the `MiningParameters` class, and only passing this class around instead of passing single parameters, like `coinbase`, `extraData`, etc... so it should help readability and make easier to manage these parameter.

More refactoring may be proposed in following PRs, to avoid making this one too big, for example `MiningParameters` could be renamed to `MiningConfiguration` for consistency with the naming of similar classes, then could make sense to pass mining parameters directly to RPC methods that update things like `coinbase`, `targetGasLimit` etc... instead of passing through other objects.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 16:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6026" class=".btn">#6026</a>
            </td>
            <td>
                <b>
                    Add trie log pruning triggered after trie log persist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu/issues/5390

TrieLogPruner loads all trie logs on startup.
Each time a trie log is persisted it is added to the "prune queue" and also the pruner is run.
Pruner executes over a pruning window (currently hardcoded to 1000) to chip away at an initially large backlog of trie logs. 
Once backlog is cleared, each prune run should just be a single trie log.

TODO:
- [x] Test with local node using smaller defaults for retain/prune window
- [ ] Add feature toggle
- [x] Feasibility of streaming all trie logs on startup? Edit: Based on [test results below](https://github.com/hyperledger/besu/pull/6026#issuecomment-1763991623) it's probably not feasible to stream all in one go for nodes with a large backlog of trielogs
- [x] Test on real nodes using current defaults: retain latest 512 blocks; backlog prune window of 1000 blocks;
- [ ] Consider an option to only prune forks
- [ ] Consider using safeBlock instead of 512 layers to retain
  - would be a nice strategy to prune only blocks older than RETAINED_LAYERS that have a subsequent finalized blockhash
- [ ] Consider belts and braces protection during rollback/forward in case pruned trielog may be in use
- [ ] Deal with "orphaned" trie logs (related to building: ones that aren't referenced in the `blockchain`; neither canonical nor a fork)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 07:42:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6023" class=".btn">#6023</a>
            </td>
            <td>
                <b>
                    Journaled world state
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

Introduce a new Journaled World State Updater, that within a transaction keeps one copy of account and storage state, restoring previous revisions on reverts and exceptional halts.  This updater only supports post-merge semantics with regard to empty accounts, namely that they do not exist in world state.

Adds an EvmConfiguration option for stacked vs journaled updater, and
wire it in where needed.  This is high touch as it's dependency
injection, but fairly simple code.

Staked and Journaled updaters both continue to exist in the codebase, with Stacked updaters being the default

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 21:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6022" class=".btn">#6022</a>
            </td>
            <td>
                <b>
                    Add bool TX pool flag to allow TX selection to avoid prioritizing TXs from the same sender
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
WIP

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6021
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 21:19:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6020" class=".btn">#6020</a>
            </td>
            <td>
                <b>
                    Transaction Validation and Selection Plugin API update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR makes some changes to the Transaction Validation and Selection Plugin API to make them more useful.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 06:03:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6017" class=".btn">#6017</a>
            </td>
            <td>
                <b>
                    Update 23.10.0 changelog
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 19:24:05 +0000 UTC
    </div>
</div>


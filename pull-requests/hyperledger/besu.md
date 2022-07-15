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
                PR <a href="https://github.com/hyperledger/besu/pull/4112" class=".btn">#4112</a>
            </td>
            <td>
                <b>
                    Update GraphQL to be closer to executioon-api spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Update GraphQL to be closer to execution-apis spec 

Update the graphQL to be closer to the execution-api specs.
This is a departure from EIP-1767 but the core devs have made it clear
that the execution-apis repo is considered canonical, not the EIP.

Major changes:
* Add support for EIP-2930 access lists
* Add support for EIP-1559 fees
* Add transaction, block, receipt, and header raw rlp fields
* Add chainID as base level query

Some items are still fake (fee estimate, effective tip).

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
        Created At 2022-07-15 00:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4107" class=".btn">#4107</a>
            </td>
            <td>
                <b>
                    [README] Add GitPOAP Badge to Display Number of Minted GitPOAPs for Contributors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Description**

Hey all, this PR adds a [GitPOAP Badge](https://docs.gitpoap.io/api#get-v1repoownernamebadge) to the README that displays the number of minted GitPOAPs for this repository by contributors to this repo.

You can see an example of this in [our Documentation repository](https://github.com/gitpoap/gitpoap-docs#gitpoap-docs).

This should help would-be contributors as well as existing contributors find out that they will/have received GitPOAPs for their contributions.

CC: @colfax23 @kayla-henrie


Signed-off-by: nixorokish

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Add GitPOAP badge to README.md

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Add GitPOAP badge to README.md

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 17:40:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4106" class=".btn">#4106</a>
            </td>
            <td>
                <b>
                    Fix PR 4098
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

There was an error during the merge from main, that readded some deleted code, fixing it

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
        Created At 2022-07-14 16:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4105" class=".btn">#4105</a>
            </td>
            <td>
                <b>
                    Remove hash to append from the queue only if the step succeeds
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

In case of an error the first hash to fetch is lost, and then the backward sync tries to go ahead and start a forward sync.
Sample log 
[first-hash-not-retry.txt](https://github.com/hyperledger/besu/files/9112753/first-hash-not-retry.txt)

This PR remove the hash from the queue only when its successfully fetched

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
        Created At 2022-07-14 14:39:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4104" class=".btn">#4104</a>
            </td>
            <td>
                <b>
                    log execution errors at right level, stops transition message propagation post-merge sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log execution errors at right level, stops transition message propagation post-merge sync


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 13:40:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4103" class=".btn">#4103</a>
            </td>
            <td>
                <b>
                    Add experimental config option to enable v5 discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
Add experimental config option to enable v5 discovery## 

## Fixed Issue(s)
fixes #4088

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 12:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4102" class=".btn">#4102</a>
            </td>
            <td>
                <b>
                    Ignore 2 tests that assume that the system language is English, if that should not be the case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description
2 of our tests that check error messages from the JVM assume that the system language is always English. If that is not the case, the JVM error messages will be localized and the tests will fail. This PR checks the system language before running those 2 tests and ignores them, if it is not English. If the system language is English the tests are executed like before.

## Fixed Issue(s)

fixes #2190

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 11:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4100" class=".btn">#4100</a>
            </td>
            <td>
                <b>
                    WIP Peer disco
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing a theory with EthPeer disconnects

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 03:56:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4099" class=".btn">#4099</a>
            </td>
            <td>
                <b>
                    Fix for RPC performance regression
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
PR #3695 uses [i.o.v.e.web.Route#blockingHandler](https://vertx.io/docs/apidocs/io/vertx/ext/web/Route.html#blockingHandler-io.vertx.core.Handler-) to attend JSON-RPC HTTP requests, but [according documentation](https://vertx.io/docs/vertx-web/java/#_using_blocking_handlers) it does it linearly. This PR adds `ordered=false` to let vert.x parallelize the processing.

## Fixed Issue(s)
fixes: #3959

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 20:26:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4098" class=".btn">#4098</a>
            </td>
            <td>
                <b>
                    Delegate all the block checks and validation to the block import phase
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

Remove preventive checks during sync, since they will be performed always performed during the import phase later, where the block will be also flagged as bad block.
With this the last failing Hive test (Invalid Ancestor Chain Re-Org, Invalid Number, Invalid P9', Reveal using sync) passes.

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
        Created At 2022-07-13 14:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4097" class=".btn">#4097</a>
            </td>
            <td>
                <b>
                    Finalised blocks should not prevent reorgs in BWS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We should allow reorgs bellow finalized blocks during Backwards Sync.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 14:00:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4096" class=".btn">#4096</a>
            </td>
            <td>
                <b>
                    Allow creating the Trie Log Layer objects outside of its package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small change to allow using the TrieLogLayer class outside its package.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 13:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4095" class=".btn">#4095</a>
            </td>
            <td>
                <b>
                    Create backward sync retries on demand
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

Currently backward sync create the max number of retries ahead of time, and this could cause unneeded retries in case of non recoverable error like in this log 
[backward-sync-retries.txt](https://github.com/hyperledger/besu/files/9101478/backward-sync-retries.txt)

This PR rework the retry strategy to create retries on demand and fast fail in case of a non recoverable exception.


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
        Created At 2022-07-13 11:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4094" class=".btn">#4094</a>
            </td>
            <td>
                <b>
                    candidate fix for missing parent worldstate
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

when we remember block after the merge we must persist the trielog. because if we lose the trielog in the memory   (ex  restart besu) we can end up in a case where the block is saved but not the trielog. this can prevent the rollback or the rollforward to work because besu will consider that it can do it as the block is present but it will failed because trielog is missing. 

may be one of the reasons for the problem found on a ropsten test node

A possible edgecase description : 
- the head is block 5
- we remember block 6
- as we remember block 6 , we save trielog 6 only in memory
- CL is saying to go to block 7
now we have
- block5 in database + trielog 5 in database
- block6 in database + trielog 6 in memory
- block7 in database + trielog 7 in database
- we have a reorg to block 6
- we rollback 7 to 6 and we persist again block 6. as trielog 6 is not in the database we save invalid trielog 6 (7->6)

 if we restart before the reorg trielog 6 is missing

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
        Created At 2022-07-13 10:55:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4093" class=".btn">#4093</a>
            </td>
            <td>
                <b>
                    Revert "Add terminal block hash and number to Ropsten genesis file (#4026)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 27fc468624d4a19067b076567ea9e1578217d34e.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Reverting this commit since it is causing error in the CL clients and needs to be implemented in a different way

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
        Created At 2022-07-13 09:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4092" class=".btn">#4092</a>
            </td>
            <td>
                <b>
                    Backward sync exception improvements
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

During the investigation of a Hive test that triggers backward sync, found some improvements that could be applied to backward sync exceptions.

1) Remove of recoursive exceptions nesting, that produces monster exception like this one
[deeply-nested-exception.txt](https://github.com/hyperledger/besu/files/9100608/deeply-nested-exception.txt)

2) Avoid to return `null` from `syncBackwardsUntil` methods in case the block is already trusted

3) Log a warning for backward sync exception that are not recoverable, likewise it is already done for recoverable exceptions

4) Rephrase the error messages when there is a validator error found during the backward sync, with the assumption that the child block is the invalid one, and the parent is correct, this makes clearer the error message for the Hive test

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
        Created At 2022-07-13 09:07:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4086" class=".btn">#4086</a>
            </td>
            <td>
                <b>
                    Enclave public key length constraint removed for private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Removes the length constraint of 44 characters for the base64 version of an enclave public key for private transactions via Tessera. More details in the linked issue.

Adapts the acceptance tests so this change could be validated against the target Tessera configuration (EC encryptor).

Upgrades package `org.web3j:eea` to 4.9.3 (it was a transitive dependency before) since the same constraint was in that package and it is used for the acceptance tests. It is the only package upgraded from the web3j suite since there is a breaking change in `PrivateTransactionManager` ([this PR](https://github.com/web3j/web3j/pull/1602/files) got rid of the `PrivateTransactionEncoder` - issue yet to be created - will update this PR with that).

## Fixed Issue(s)

fixes #3819 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 10:50:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4085" class=".btn">#4085</a>
            </td>
            <td>
                <b>
                    checkpoint sync for merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamChupa</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

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
        Created At 2022-07-12 08:36:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4083" class=".btn">#4083</a>
            </td>
            <td>
                <b>
                    host header parse error
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
fixes the parsing of host headers. adds test coverage for this case on both http and websockets.

## Fixed Issue(s)
#4082 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 20:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4080" class=".btn">#4080</a>
            </td>
            <td>
                <b>
                    New payload: add invalid to bad blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
If a block is deemed invalid, because it did not descend from the terminal block, we add it to our bad blocks. This is a fix for the failing Hive engine test `Transition to a Chain with Invalid Terminal Block, Lower Configured Total Difficulty (Transition Payload)`.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 10:53:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4078" class=".btn">#4078</a>
            </td>
            <td>
                <b>
                    Fix transition protocol schedule
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
        Created At 2022-07-08 17:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4077" class=".btn">#4077</a>
            </td>
            <td>
                <b>
                    Release 22.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.4.4

cherry picks from main:
49e4fd860 -> worldstate not avail (#4069)
6aa88129e -> stateroot mismatch (#4041)
043191a40 -> jwt auth on websockets (#4039)
90f891b78 -> do not move head on exec and propose (#4013)
b5fa62c0b -> sync check before processing remote transactions (4035)
3baa4da99 -> upgrade for websockets (#4019)
5024c0788 -> sepolia TTD (#4024)
5ee9be837 -> heal step in snap (#3920)
261b1e03f -> remove peer block height requirements (#3911)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 15:32:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4075" class=".btn">#4075</a>
            </td>
            <td>
                <b>
                    Otel take 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fixes the OpenTelemetry configuration so it doesn't initialize the global opentelemetry singleton when getting the tracer.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 11:38:04 +0000 UTC
    </div>
</div>


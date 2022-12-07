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
                PR <a href="https://github.com/hyperledger/besu/pull/4782" class=".btn">#4782</a>
            </td>
            <td>
                <b>
                    Moved besu docs devs to emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moving two besu docs developers from the besu maintaners group to emeritus status.
@bgravenorst and @NicolasMassart 

Now that the besu-docs have moved to separate repo, this access can be separated. 
The docs repo uses some of the same groups https://github.com/hyperledger/besu-docs/settings/access
but the maintainers one is different https://github.com/orgs/hyperledger/teams/besu-docs-maintainers/members

For besu repos, `triage` is fine. Besu docs developers have to be able to update PRs like adding labels or updating description so that the doc work is easier when the code PR is not detailed enough. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 21:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4781" class=".btn">#4781</a>
            </td>
            <td>
                <b>
                    EIP-4750 EOF Functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

WIP - do not commit

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
        Created At 2022-12-05 20:41:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4780" class=".btn">#4780</a>
            </td>
            <td>
                <b>
                    Speedup modexp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Speed up the gas calculation and execution of the modexp precompile.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 18:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4778" class=".btn">#4778</a>
            </td>
            <td>
                <b>
                    Add support for another Transaction Encoder/Decoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transaction Encoder/Decoder automatically implied RLP encoding. The 4844 Blob Transaction should be encoded with SSZ encoding.

This PR is a suggestion how to refactor the Encoder to support multiple different types of encodings.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 16:19:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4775" class=".btn">#4775</a>
            </td>
            <td>
                <b>
                    Changed chain download error log level from error to debug.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Change the log level for a common chain download error from `error` to `debug`.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4081 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 15:20:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4773" class=".btn">#4773</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.10.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.10.3-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-03 15:44:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4772" class=".btn">#4772</a>
            </td>
            <td>
                <b>
                    Release 22.10.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.10.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-03 15:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4771" class=".btn">#4771</a>
            </td>
            <td>
                <b>
                    subscribe prior to getting stateTrieNode in cacheStorageNodes
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
ensure storage caching subscribes before accessing worldstate at all

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4765 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 23:35:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4769" class=".btn">#4769</a>
            </td>
            <td>
                <b>
                    prep changelog for 22.10.2
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
add changelog description for 22.10.2 hotfix

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
        Created At 2022-12-02 22:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4767" class=".btn">#4767</a>
            </td>
            <td>
                <b>
                    Ensure that Snashot worldstates remain open for async operations
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
in 22.10.1, two new operations pre-load account and storage from their respective worldstate asynchronously.  If the worldstate is based on a snapshot, there is a race where the snapshot might be closed ahead of the async operations completing, and subsequently result in a segfault when trying to access a closed rocksdb snapshot.  

This PR adds a subscriber implementation for BonsaiWorldStateKeyValueStorage which ensures that the storage will not be closed while subscribers are still operating on it.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4765 
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 16:14:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4762" class=".btn">#4762</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.10.2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.10.2-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 22:28:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4761" class=".btn">#4761</a>
            </td>
            <td>
                <b>
                    Release 22.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.10.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 22:04:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4760" class=".btn">#4760</a>
            </td>
            <td>
                <b>
                    Add EIP-4200: EOF - Static relative jumps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
This PR adds support for [EIP-4200](https://eips.ethereum.org/EIPS/eip-4200): EOF - Static relative jumps

Note: this EIP has been CIF'd but the spec isn't stable yet, I think mostly regarding to the gast cost of the operations (check the _Gas costs overview_ section from the [Spec-level Open Issues](https://notes.ethereum.org/@ipsilon/eof1-checklist#Spec-level-Open-Issues) notes for Shangai). Until then I think it's better to keep it as draft

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 20:41:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4759" class=".btn">#4759</a>
            </td>
            <td>
                <b>
                    Move connect decision into protocol layer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 08:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4758" class=".btn">#4758</a>
            </td>
            <td>
                <b>
                    Withdrawals and timestamp
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
DO NOT MERGE

Test branch for withdrawals & timestamp protocol schedule changes

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
        Created At 2022-12-01 07:21:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4757" class=".btn">#4757</a>
            </td>
            <td>
                <b>
                    Use value comparisons instead of reference comparisons in some places
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Change three reference comparisons that I believe should be value comparisons.

* Comparisons with `Bytes.EMPTY` will not work as expected.
  * For example, `Bytes.of() == Bytes.EMPTY` is false.
* While the two implementations are enums, `MetricCategory` is actually an interface.
  * In practice this is fine, but it's safer for this to be a value comparison.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 21:27:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4756" class=".btn">#4756</a>
            </td>
            <td>
                <b>
                    Mul speedup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Move mul from UInt256 wrapping to direct BigInteger math.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

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
        Created At 2022-11-30 16:45:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4754" class=".btn">#4754</a>
            </td>
            <td>
                <b>
                    Replace errorprone-checks with consensys/errorprone-checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR replaces the internal errorprone-checks with the external [consensys/errorprone-checks](https://github.com/ConsenSys/errorprone-checks) that Teku & Discovery use. It contains all of the same checks plus a few new ones. I think it's a good idea to deduplicate this stuff. In subsequent PRs, I'll review & enable some of those new checks.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 15:54:04 +0000 UTC
    </div>
</div>


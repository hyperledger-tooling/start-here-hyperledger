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
                PR <a href="https://github.com/hyperledger/besu/pull/3655" class=".btn">#3655</a>
            </td>
            <td>
                <b>
                    Fast sync with merge
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 12:21:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3654" class=".btn">#3654</a>
            </td>
            <td>
                <b>
                    clarify logging of wait for peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

clarify log messages

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 10:51:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3652" class=".btn">#3652</a>
            </td>
            <td>
                <b>
                    Rename blacklist -> denylist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

internal variables only. no external changes required.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 05:35:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3649" class=".btn">#3649</a>
            </td>
            <td>
                <b>
                    Changelog typos
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
        Created At 2022-03-29 22:34:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3647" class=".btn">#3647</a>
            </td>
            <td>
                <b>
                    Updated jackson-databind to version 2.13.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Previsous jackson-databing version has been flagged (https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-36518).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 21:26:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3645" class=".btn">#3645</a>
            </td>
            <td>
                <b>
                    Fix nullpointer on bonsai trie
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

This PR modify the bonsai implementation in order to avoid having nullpointer exception . This PR ils related to this issue https://github.com/hyperledger/besu/issues/3644

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
        Created At 2022-03-29 09:20:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3638" class=".btn">#3638</a>
            </td>
            <td>
                <b>
                    Improving backwards sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous implementation of backward sync only saved the headers and block bodies to disk. This PR combines the structure of backward sync chain into one dequeue, together with storing the chain on the disk and retrieving it back. 

This is an intermediate change before a stage where the majority of Backward sync will be stored on disk most of the time. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 21:48:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3636" class=".btn">#3636</a>
            </td>
            <td>
                <b>
                    delete slice input data code
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
This code do not check whether the input value is not empty array. So, I changed this code as follows, I tried to connect the errors to EnclaveClientException.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3635

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 05:00:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3634" class=".btn">#3634</a>
            </td>
            <td>
                <b>
                    update rocksdbjni to v6.29.4 for compatibility with arm64 CPU architecture
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
Updates rocksdbjni dependency to v6.29.4 for compatibility with arm64 CPU architecture. 
It was tested on Apple M1 Pro 2021, OSx 12.3 

## Related Issue(s)
- #3540 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 23:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3633" class=".btn">#3633</a>
            </td>
            <td>
                <b>
                    Update reference tests to 0e8d25bb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## Fixed Issue(s)
fixes #3632 

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 22:37:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3631" class=".btn">#3631</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Performance test : bloom filter test
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
Performance test :
Enable RocksDB Bloom filter.

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
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
        Created At 2022-03-25 13:24:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3629" class=".btn">#3629</a>
            </td>
            <td>
                <b>
                    Update the PR template to include a documentation checklist item.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: bgravenorst <byron.gravenorst@consensys.net>

## PR description
Updated the GitHub PR template to include a documentation checklist item.

## Fixed Issue(s)
Fixes #3628 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 01:44:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3626" class=".btn">#3626</a>
            </td>
            <td>
                <b>
                    Skip seen transactions
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

This is the last PR in the series to review and optimize transaction synchronization, and its goal is to avoid reprocessing transactions, that Besu have already seen recently.

The currently way Besu has to spot if a transaction has already been process, is to look if the transaction is present in the transaction pool, that by default is 4K, while the amount of pending transactions on the mainnet, is much more, the order of hundred of thousands, so basically even if a transaction has been already processed, the chances that it gets reprocessed is very high, with the result of doing a lot of useless work, that affects Besu performance.

A trivial solution could be to just raise the transaction pool size, but that is not always advisable, because it is critical for block production to keep it fast, and incresing its size could negatively affect the perfomance of the strategy choosen to select transactions to include in the block.

A better option, implemented in this PR, is to leverage data that we already have, and that keeps the history of the transactions exchanged with other peers. This data is just a collection of transaction hashes that we have received or seen, and in any case if a transaction is in that collection, it means that it has already been processed by Besu, so it is possible to directly skip it.

Tests show a reduced CPU usage:
![image](https://user-images.githubusercontent.com/91944855/159903502-35ad0aff-bfc8-4ab0-98c7-c0fdbc2503a5.png)
![image](https://user-images.githubusercontent.com/91944855/159903608-57ea1bdc-332f-42fc-aa35-7c3021e30d29.png)

due to the much less turnover in the transaction pool
![image](https://user-images.githubusercontent.com/91944855/159903959-c4bc1de1-ee3e-45ed-8f2f-6149a885a070.png)
![image](https://user-images.githubusercontent.com/91944855/159904240-adafdd71-4ad9-4f7b-8782-3770fb3f9479.png)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 17:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3625" class=".btn">#3625</a>
            </td>
            <td>
                <b>
                    init object for snapsync pipeline
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

This is the first step initializing the snapsync pipeline. Setting up utility objects and request classes. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 15:27:49 +0000 UTC
    </div>
</div>


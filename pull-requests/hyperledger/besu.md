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
                PR <a href="https://github.com/hyperledger/besu/pull/5060" class=".btn">#5060</a>
            </td>
            <td>
                <b>
                    Update GitHub pull request template (non-mainnet AT)
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
Update Github pull request template to add option to advise to run non-mainnet test if required.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Related to #4921 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 01:48:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5059" class=".btn">#5059</a>
            </td>
            <td>
                <b>
                    Add worldstate heal mechanism 
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

This PR add a heal  mechanism fo the worldtstate in case of inconsistency (unable to trie node). To fix this, we start a quick heal of the worldstate automatically and once the fix is done we restart the block import.

After the detection of an invalid path
- we delete this path to force the healing of this part.
- then we delete the trielogs. 
- we select a pivot block (before of after the heal)
- we move the blokchain to this pivot block (rewind or download the missing blocks) 
- then we launch a worldstate heal. 


This feature can also heal a node that has been inconsistent for a long time, but it will take longer because there will be more nodes to heal.  With this PR the healing will be done as soon as the problem is detected so there will not a lot to heal and it will be fast

## Performed tests
 - Trigger multiple inconsistencies to fix  (passed)
 - Fixed a node that has been inconsistent for a long time (passed)
 - Run a snapsync from scratch on goerli (passed)
 - Run a checkpoint sync from scratch on goelri (passed)
 - Run a checkpoint sync from scratch on main **(in progress)**
 - Run a validator teku+besu on goerli (passed)
 - Profile performance on this node to avoid perf regression (passed)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

#4379 
#4785 
#4768

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 07:22:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5057" class=".btn">#5057</a>
            </td>
            <td>
                <b>
                    Include withdrawals tests in ref tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Include withdrawal tests in EIPTests as part of the reference tests.

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
        Created At 2023-02-05 22:53:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5055" class=".btn">#5055</a>
            </td>
            <td>
                <b>
                    EIP-6110: Handle validator deposits in EL
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

Appends validator deposits to the Execution Layer block structure: [EIP-6110](https://eips.ethereum.org/EIPS/eip-6110)

## Fixed Issue(s)
#5004 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 06:54:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5054" class=".btn">#5054</a>
            </td>
            <td>
                <b>
                    Adds to 22.10.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Additions to 22.10.4 release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 01:13:24 +0000 UTC
    </div>
</div>


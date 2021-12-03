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
                PR <a href="https://github.com/hyperledger/besu/pull/3123" class=".btn">#3123</a>
            </td>
            <td>
                <b>
                    Move discovery options constants to genesis files of predefined networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR is a continuation of #2944 by moving the hardcoded discovery values into each of the genesis files.
  * a2b081e01 has the minimal set of changes for the _factory method_ of `org.hyperledger.besu.cli.config.EthNetworkConfig` to resolve the bootnodes and dns from the genesis file. The _factory method_ could have been removed and its behavior integrated directly into the `org.hyperledger.besu.cli.BesuCommand` reusing the logic for external genesis files, but that would have impacted in many tests, making the review harder to perform.
  * efaf0ca39 and c12da44ca are not mandatory for this PR but I think it would be hard to make this changes as part of a bigger and meaningful PR. Can be removed if any reviewer request it.
 
It's worth to mention that the hardcoded discovery values were keep just for testing purposes within that scope.

## Enhacement(s)
closes #3113
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 03:40:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3121" class=".btn">#3121</a>
            </td>
            <td>
                <b>
                    WIP || (internal) Refactor hard coded state roots in PrivacyReorgTest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
We're generating the state roots at test time without assuming the seed value or random algorithm used in BlockDataGenerator

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #1793 

## Changelog
Not required (test code refactor)

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 09:43:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3120" class=".btn">#3120</a>
            </td>
            <td>
                <b>
                    Add Frank Li as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Frank has made more than 5 significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Afrankisawesome+is%3Aclosed) that improved the quality of Besu and/or added new features.

Voting ends 2 weeks from the publication of this PR or once more than 50% of the current maintainers approved.

For more information on this process see the **Becoming a Maintainer** section in the MAINTAINERS.md file.

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 03:56:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3119" class=".btn">#3119</a>
            </td>
            <td>
                <b>
                    Emeritus maintainers x 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving the following maintainers to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity during Q3/Q4 2021 (since July 2021):
* @mbaxter’s last Besu activity was in July 2021
* @abdelhamidbakhta’s last Besu activity was in July 2021

We very much appreciate their contributions but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.
This vote is open until either an absolute majority of active maintainers votes for the same outcome, or until two weeks has passed, after which a voting majority will determine the outcome (with a tie resulting in no change).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 23:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3118" class=".btn">#3118</a>
            </td>
            <td>
                <b>
                    Start external services before we start plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description - start external services before we start plugins

Reasons:

- you may wish to query the current state of your blockchain using rpc before you start processing new blocks

- you may wish to register a websocket e.g to listen for blocks currently, you will probably miss one because we start processing before we start the ws service

To enable this a 'beforeExternalServices' hook was addedd to allow plugins to do things before those services are started. 

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 15:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3117" class=".btn">#3117</a>
            </td>
            <td>
                <b>
                    QBFT migration: Create a switchable protocol context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
For the QBFT migration we need to be able to return the appropriate consensus context for the current consensus mechanism.

This introduces a schedulable protocol context and scheduable context that are used together to return the consensus context for the current chain height.

Fixes #3000 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 06:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3116" class=".btn">#3116</a>
            </td>
            <td>
                <b>
                    fix flakey test caused by random payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes flakey tests e.g. https://app.circleci.com/pipelines/github/hyperledger/besu/11940/workflows/7dc4c157-f51b-4ba7-aaa8-3baec6b5a038/jobs/65476/tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 05:45:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3114" class=".btn">#3114</a>
            </td>
            <td>
                <b>
                    Reduce log level down to debug on EthPeer Permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce log level down to debug on EthPeer Permissioning - the logs can become very verbose when blocking p2p transactions in private networks.

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 16:04:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3112" class=".btn">#3112</a>
            </td>
            <td>
                <b>
                    Include invalid value in Enode error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Makes it much easier for users to identify their mistake if the CLI argument after `--bootnodes <some-valid-enode>` has a typo. PicoCLI will treat any unrecognised option as another bootnode so it's very confusing to get an invalid enode message when the enode is fine and it's the next argument that's incorrect.

For example `--bootnodes enode://blah@127.0.0.1:30303 --datapath foo` would otherwise print an error message saying there wasn't an `enode://` prefix when there clearly is.  When the invalid value is shown the user can see that it's actually `--datapath` that's unrecognised and fix the problem.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 09:37:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3111" class=".btn">#3111</a>
            </td>
            <td>
                <b>
                    Eip 4399
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

Implements EIP-4399 by repurposing the DIFFICULTY opcode to provide entropy provided by beacon chain post merge.

This is intended to change the behavior during the merge, and leaving the semantic changes to clarify this behavior till after the merge, when the opcode can be documented as renamed to RANDOM, thought its instruction byte remains the same.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-28 04:50:05 +0000 UTC
    </div>
</div>


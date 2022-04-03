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
                PR <a href="https://github.com/hyperledger/besu/pull/3675" class=".btn">#3675</a>
            </td>
            <td>
                <b>
                    Upgrade OpenTelemetry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Upgrades OpenTelemetry to the latest version, and make sure we configure the SDK with environment variables.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-03 06:51:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3674" class=".btn">#3674</a>
            </td>
            <td>
                <b>
                    Remove Gas object and replace with primitive long
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove the Gas object from the EVM and replace it with the primitive
long. This will have positive impact on short lived object garbage
collection stats, which at very high load causes significant performance
issues.

This also codifies EIP-4803 in the Besu EVM, limiting gas to a signed
64-bit long internally.

There was one notable issue with this transition. Some reference tests
push the limits of memory expansion which results in gas costs over the
EIP limit. The solution is to "clamp" such addition and multiplication
operations at the max or min long value, resulting in the out-of-gas
check failing (such operations will never have a valid execution with
max gas remaining).

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

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
        Created At 2022-04-01 14:07:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3671" class=".btn">#3671</a>
            </td>
            <td>
                <b>
                    Fix block import subcommand by r
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some instantiation of `CommandLine` were throwing errors, because the were not using `BesuCommandCustomFactory` to create the necessary `VersionProvider`, which is a recent requirement for subcommands.

Instead of creating new `CommandLine`instances, the PR reuses the existing objects, which are already correctly configured.

Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
fixes #3646

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 14:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3669" class=".btn">#3669</a>
            </td>
            <td>
                <b>
                    [MINOR] Rename peer deny list + slight log change
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
Changes the PeerReputationManager class to PeerDenylistManager to better reflect the class purpose

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 08:52:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3667" class=".btn">#3667</a>
            </td>
            <td>
                <b>
                    Improve code readability
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
        Created At 2022-03-31 08:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3664" class=".btn">#3664</a>
            </td>
            <td>
                <b>
                    FlexiblePrivacyPrecompile - Handle invalid Payload ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Handle the case where payloadId passed in is null or < 32 bytes. 

See #3635 

Added 2 new tests for null and < 32bytes

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 06:33:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3663" class=".btn">#3663</a>
            </td>
            <td>
                <b>
                    update after releasing 22.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 04:52:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3662" class=".btn">#3662</a>
            </td>
            <td>
                <b>
                    Graphql - allow null topic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow creation of LogTopic from null
* modify graphql spec to allow null values in list of topics
* added test file with null topic in filter to match any topic
This means graphql now matches http behaviour and also matches what we have documented https://besu.hyperledger.org/en/stable/Concepts/Events-and-Logs/#topic-filters

Fixes #3519

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 04:32:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3661" class=".btn">#3661</a>
            </td>
            <td>
                <b>
                    prepare for release 22.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.1.3

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 03:27:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3658" class=".btn">#3658</a>
            </td>
            <td>
                <b>
                    useful peers log message changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Clarify messages around "no useful peers found" 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 23:25:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3657" class=".btn">#3657</a>
            </td>
            <td>
                <b>
                    handle jwt keys with either 0x or not
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 15:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3656" class=".btn">#3656</a>
            </td>
            <td>
                <b>
                    Add snap pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">snapsync</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR adds the majority of  classes related to the snapsync pipeline. More tests will be added later.
There will be a dedicated PR to delete hard values in order to add configuration flags 

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
        Created At 2022-03-30 13:50:53 +0000 UTC
    </div>
</div>

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


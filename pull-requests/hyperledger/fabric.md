---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4713" class=".btn">#4713</a>
            </td>
            <td>
                <b>
                    hyperledger#2814
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update

#### Description
Example json file for CouchDb index doesn't exist anymore. Hence updating referece to valid json file as mentioned in other file of documentation.

#### Additional details
Broken json file reference can be found [here](https://hyperledger-fabric.readthedocs.io/en/latest/private-data-arch.html#using-indexes-with-collections)
New json file reference is taken from [here](https://hyperledger-fabric.readthedocs.io/en/latest/couchdb_as_state_database.html#couchdb-indexes)

#### Related issues
[hyperledger-fabric#2814](https://github.com/hyperledger/fabric/issues/2814)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-02 14:03:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4712" class=".btn">#4712</a>
            </td>
            <td>
                <b>
                    Update readme for LTS versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update readme for LTS versions

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 17:35:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4711" class=".btn">#4711</a>
            </td>
            <td>
                <b>
                    Update readme for LTS versions (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update readme for LTS versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 17:32:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4710" class=".btn">#4710</a>
            </td>
            <td>
                <b>
                    Update readme for LTS versions (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update readme for LTS versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 17:15:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4707" class=".btn">#4707</a>
            </td>
            <td>
                <b>
                    Fix test flake in TestImpatientStreamDetectSelf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The implementation of the fake/mock orderer in the unit tests reads a seek envelope and the test fails if reading fails.

When the `TestImpatientStreamDetectSelf` test ends, it shuts down the fake orderer, and as a result, reading from the stream fails and the test fails also.

This commit simply short-circuits the test to avoid reading from the stream, but planting an error before establishing the stream, as reading from the stream is not needed for the test but only establishing it in order to get the TLS certificate.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 18:06:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4706" class=".btn">#4706</a>
            </td>
            <td>
                <b>
                    Add a doc notice that old version  is no longer supported (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This notice will be added to every rst page, including the welcome page.
It will not be added to the md pages, but most of the landing pages are rst.

Also update the README accordingly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 18:01:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4705" class=".btn">#4705</a>
            </td>
            <td>
                <b>
                    Test flake in BFTDeliverer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Test update

#### Description

Prevent a test flake in BFTDeliverer unit tests

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 14:47:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4704" class=".btn">#4704</a>
            </td>
            <td>
                <b>
                    BFT chain unit tests: successful tx propagation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

The purpose of this PR is to create BFT chain unit tests.
The first step is to create an active chain using mocks, the second step is to start a network of 4 nodes and the third is to ensure a successful tx propagation.

#### Related issues

issue #4008 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 10:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4703" class=".btn">#4703</a>
            </td>
            <td>
                <b>
                    Update documentation on event services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

This patch updates descriptions in the documentation to shift focus from legacy SDKs to Gateway API.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related PRs
- https://github.com/hyperledger/fabric/pull/3219
- https://github.com/hyperledger/fabric/pull/4221

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 00:34:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4702" class=".btn">#4702</a>
            </td>
            <td>
                <b>
                    Check env variable before using it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I5167afca9352b5bdc7d96dbe7e9ef25e2e2db69e

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

When the TARGET env variable is not set, the script will fail to run. 

This patchset adds the checking and ouputs useful hints.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 19:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4700" class=".btn">#4700</a>
            </td>
            <td>
                <b>
                    Fix some typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

This patch fixes some typos.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 03:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4699" class=".btn">#4699</a>
            </td>
            <td>
                <b>
                    Update footer.html
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

This patch updates year 2023 to 2024 in footer.html.
<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 01:37:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4695" class=".btn">#4695</a>
            </td>
            <td>
                <b>
                    BFT: A BFT synchronizer for smartbft
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- New feature

#### Description

A BFT synchronizer for smartbft

#### Related issues

Issue #4566 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-25 13:55:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4694" class=".btn">#4694</a>
            </td>
            <td>
                <b>
                    Excessive mutex locks were removed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by fubss <ivanlaish@gmail.com>

# Removing excessive mutex locks increasing performance

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

As part of my research [Uncovering the Perfect Scalable Database for Hyperledger Fabric's Evolution](https://ieeexplore.ieee.org/document/10189331) it was discovered that the Hyperledger Fabric peer node does not use resources at 100% for some types of transactions. One of the reasons of it is the often mutexes locks in the source.

This change removes three excessive mutexes locks. Some of them were locking already atomic operations and some were locking nothing.


#### Additional details

<!--- Additional implementation details or comments to reviewers. -->

The results of the peer node performance improvement were published in the paper provided above. The change has given better CPU and Disk usage and increased transaction per second rate.

Performance benchmarks of peer node were made with hyperledger-caliper. The results for write operation are:

  * for 100 byte transactions:

    * TPS rate increased to 5% 

    * CPU usage increased to 7%

    * Disk Write rate increased to 5%

  * for 4000 byte transactions:

    * TPS rate increased to 5% 

    * CPU usage increased to 6%

    * Disk Write rate increased to 4%

  * for 64000 byte transactions:

    * TPS rate increased to 2% 

    * CPU usage stayed the same

    * Disk Write rate increased to 1%

Full Caliper reports are availiable [here](https://drive.google.com/drive/folders/15eOiYOG7QeLv-qj5A5RNHWLNRwf2xduo?usp=sharing). For read operation no performance changes were detected.

The changes were sucessfully tested locally and with GitHub CI/CD.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-25 13:11:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4693" class=".btn">#4693</a>
            </td>
            <td>
                <b>
                    BFT: skip self-endpoint when pulling blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Change-Id: Ia183eef4f263943d5f387e8156d450790bee5cb2
#### Type of change

- New feature

#### Description

The orderer source provides a set of orderers to connect to, and is used by the BFTDeliverer. The BFTDeliverer is employed in the peer and in the orderer. When used in the orderer, it should skip the self-endpoint. In this commit we allow the orderer source to be set with the self-endpoint, and thus allow it to skip it when providing a set of orderers to pull blocks from.

#### Related issues

Issue #4566 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-25 10:12:07 +0000 UTC
    </div>
</div>


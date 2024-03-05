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
                PR <a href="https://github.com/hyperledger/fabric/pull/4720" class=".btn">#4720</a>
            </td>
            <td>
                <b>
                    BFT header receiver verifies config blocks in full
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Once a header receiver discovers it has a config block rather then a block attestation, it will verify the block in full, i.e. including the data hash.

#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 09:12:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4717" class=".btn">#4717</a>
            </td>
            <td>
                <b>
                    Set leader rotation disabled but make it possible later
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The current code sets leader election disabled by hardcoding it. More specifically, it overrides leader rotation in the code section that parses the config. This means that if we choose to make it possible to enable it at a later version, it won't be possible to run mixed versions of v3.0.

This commit makes sure that if we decide to permit leader rotation later on, it will be possible if the majority of nodes desire so.

It achieves this by disabling leader rotation in two places:
- Channel creation
- Validation of config update transactions

However, the config parsing logic now honors leader election if it's enabled in the channel config.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 16:37:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4716" class=".btn">#4716</a>
            </td>
            <td>
                <b>
                    Disable vulnerability scans for v2.2 and v2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fabric has recently ended maintenance of v2.2 and will no longer backport dependency updates to v2.2 or v2.4. 

All users are encouraged to use v2.5 at this point, therefore just run the vulnerability scan for v2.5 and main branches.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 15:53:09 +0000 UTC
    </div>
</div>

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

Support for stopping a node and restarting the network has been added. 

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


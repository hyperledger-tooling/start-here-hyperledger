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
                PR <a href="https://github.com/hyperledger/fabric/pull/4857" class=".btn">#4857</a>
            </td>
            <td>
                <b>
                    Bump github.com/hyperledger/fabric-lib-go to v1.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/hyperledger/fabric-lib-go to v1.1.2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 18:09:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4856" class=".btn">#4856</a>
            </td>
            <td>
                <b>
                    Allow the peer delivery client to select policy
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

Issue: #4847

#### Related issues

#4847
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-12 16:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4855" class=".btn">#4855</a>
            </td>
            <td>
                <b>
                    Fix docs reference version of hyperledger-fabric-ca from 1.4 to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Last LTS version **[release-1.4](https://github.com/hyperledger/fabric-ca/tree/release-1.4)** of **hyperledger-fabric-ca** was abandoned 4 years ago, but the successor version **1.5** has never been present as a candidate in the [public docs page](https://hyperledger-fabric-ca.readthedocs.io/en/latest/). Instead, the hyperledger-fabric-ca team only update **latest** version.

#### Type of change

- Documentation update

#### Description
To adapt **hyperledger-fabric-ca** docs version, rename all references to hyperledger-fabric-ca version **release-1.4** (if present) to **latest**, namely, change https://hyperledger-fabric-ca.readthedocs.io/en/release-1.4 to https://hyperledger-fabric-ca.readthedocs.io/en/latest. Because **hyperledger-fabric-ca** docs version **release-1.4** hasn't been updated for 4 years, and the public maintaining version is **latest**.

#### Additional details

Updated docs is built out for review: https://ethan-li-fabric.readthedocs.io/en/latest/

#### Related issues

#4854 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-11 01:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4852" class=".btn">#4852</a>
            </td>
            <td>
                <b>
                    chore: fix comments
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
        Created At 2024-05-10 02:03:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4851" class=".btn">#4851</a>
            </td>
            <td>
                <b>
                    Add OpenSSF Scorecard bug
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

Add the Scorecard bug to the Readme.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 22:26:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4850" class=".btn">#4850</a>
            </td>
            <td>
                <b>
                    Update channel_update_tutorial.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is two 'use' in the text. Deleting one of them.

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

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
        Created At 2024-05-09 17:33:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4849" class=".btn">#4849</a>
            </td>
            <td>
                <b>
                    Add logging spec for integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add logging spec for integration tests so that it can
be edited when troubleshooting specific tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 16:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4848" class=".btn">#4848</a>
            </td>
            <td>
                <b>
                    Improve softhsm test guidance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs for softhsm integration tests.
Add log message when softhsm tests don't execute.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 16:48:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4846" class=".btn">#4846</a>
            </td>
            <td>
                <b>
                    Update ordering service docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove references to Kafka.
- Mention CFT and BFT options.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 15:08:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4845" class=".btn">#4845</a>
            </td>
            <td>
                <b>
                    Bump jinja to 3.1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump jinja to 3.1.4.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 13:19:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4844" class=".btn">#4844</a>
            </td>
            <td>
                <b>
                    Publish OpenSSF scorecard results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've found that fabric scorecard is already published at https://scorecard.dev/viewer/?uri=github.com/hyperledger/fabric

Publishing from our own github action will at least give us control over the scorecard execution and publishing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 12:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4843" class=".btn">#4843</a>
            </td>
            <td>
                <b>
                    Add GHA permission to broken link checker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Every github action should have top level permission set to read.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 12:52:44 +0000 UTC
    </div>
</div>


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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4842" class=".btn">#4842</a>
            </td>
            <td>
                <b>
                    update staticcheck version (backport #4840)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrate staticcheck version to latest release.
The current version breaks with go 1.22, so cannot be used locally when go 1.22 is installed. see https://staticcheck.io/changes/2023.1/#2023.1.7

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 16:08:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4841" class=".btn">#4841</a>
            </td>
            <td>
                <b>
                    Doc tutorials - Remove double quotes for env variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Double quotes are problematic in some environments, see https://github.com/hyperledger/fabric/issues/4358.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 14:45:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4840" class=".btn">#4840</a>
            </td>
            <td>
                <b>
                    update staticcheck version
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

Upgrate staticcheck version to latest release.
The current version breaks with go 1.22, so cannot be used locally when  go 1.22 is installed.
see https://staticcheck.io/changes/2023.1/#2023.1.7

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 13:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4839" class=".btn">#4839</a>
            </td>
            <td>
                <b>
                    Remove guidance on Docker Desktop version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docker Desktop 2.5.0.1 is now outdated.
There have not been problems reported in recent versions of Docker Desktop.
We can fallback to the "prereq" doc topic that states to use the latest version.

Closes #4833

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 13:37:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4838" class=".btn">#4838</a>
            </td>
            <td>
                <b>
                    test flake bft deliverer
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

Removing a test flake

#### Related issues

#4832 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 13:18:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4834" class=".btn">#4834</a>
            </td>
            <td>
                <b>
                    Remove Idemixgen from Fabric produced binaries
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
Removed Idemixgen from the documentation to reflect its removal from the set of Fabric produced binaries.

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

Closes https://github.com/hyperledger/fabric/issues/3575

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
        Created At 2024-05-03 14:14:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4831" class=".btn">#4831</a>
            </td>
            <td>
                <b>
                    Create scorecard.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run OpenSSF Scorecard report weekly.
Scorecard details available at https://securityscorecards.dev/.

The results will not yet be published to OpenSSF
`(publish_results: false)`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 17:45:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4830" class=".btn">#4830</a>
            </td>
            <td>
                <b>
                    Suppress scheduled jobs on personal forks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Suppress scheduled jobs on personal forks.

Also, enable running the jobs on-demand in personal forks by using a runner that is available on personal forks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 16:39:31 +0000 UTC
    </div>
</div>


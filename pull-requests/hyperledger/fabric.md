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
                PR <a href="https://github.com/hyperledger/fabric/pull/4690" class=".btn">#4690</a>
            </td>
            <td>
                <b>
                    Add missing procedures to couchdb_tutorial.rst
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

This patch adds missing procedures to couchdb_tutorial.rst

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

Resolves #4677

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
        Created At 2024-02-21 05:33:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4689" class=".btn">#4689</a>
            </td>
            <td>
                <b>
                    Allow error to be wrapped
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I3620094d9aece9151bf5dd08005673c2610aa041

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Change output fmt from %s to %w, which is supported by errors and fmt 
to wrap error.


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
        Created At 2024-02-20 16:16:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4687" class=".btn">#4687</a>
            </td>
            <td>
                <b>
                    Add ledgerutil to docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All ledgerutil to docs.
Also remove idemixgen since it was moved to its own repository.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 18:42:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4686" class=".btn">#4686</a>
            </td>
            <td>
                <b>
                    Catch up installation procedures in main to v2.5.6
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

- Documentation update

#### Description

Since the install procedures in the documentation for each version refer to the install scripts in the main repository, the install scripts in the main repository should also be updated to catch up with v2.5.6.

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
        Created At 2024-02-19 09:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4685" class=".btn">#4685</a>
            </td>
            <td>
                <b>
                    Detect your own endpoint in HeightsByEndpoints()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, when an orderer node chooses a single node endpoint to pull blocks from (and the rest to pull headers from), it may pick itself, which is a problem because this endpoint will never bring it any blocks since it is itself.

This commit makes the function HeightsByEndpoint return the endpoint of yourself, such that the caller can filter it out.

The identification of your own endpoint is done by looking at the TLS certificate of the remote node and comparing it with your own.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 08:53:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4684" class=".btn">#4684</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.2.15.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 02:43:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4683" class=".btn">#4683</a>
            </td>
            <td>
                <b>
                    Release commit for v2.5.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add docs and release notes for v2.5.6 release.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 02:26:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4682" class=".btn">#4682</a>
            </td>
            <td>
                <b>
                    Use fabric-lib-go v1.1.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transition from the fabric-lib-go temporary branch to the actual release v1.1.0.

This is the release that includes the common
bccsp, metrics, and flogging packages that
are shared across fabric and fabric-ca.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 14:36:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4681" class=".btn">#4681</a>
            </td>
            <td>
                <b>
                    Improve validation and command docs for queryapproved
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)
- Documentation update

#### Description

This patch ensures 'sequence' is not specified without 'name', adding clarity and preventing user confusion.
This also includes minor improvements on the command reference.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

https://github.com/hyperledger/fabric/issues/4564

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
        Created At 2024-02-16 07:52:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4680" class=".btn">#4680</a>
            </td>
            <td>
                <b>
                    up consensus library
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
        Created At 2024-02-15 05:52:37 +0000 UTC
    </div>
</div>


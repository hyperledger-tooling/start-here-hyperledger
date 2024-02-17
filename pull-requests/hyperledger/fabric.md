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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4679" class=".btn">#4679</a>
            </td>
            <td>
                <b>
                    BFT chain unit tests: create a new chain without errors
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
The first step is to create an active chain using mocks. 

#### Related issues

issue #4008 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 15:35:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4678" class=".btn">#4678</a>
            </td>
            <td>
                <b>
                    Switch to bccsp, metrics, flogging in fabric-lib-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following packages are being moved from fabric to fabric-lib-go so that they can be shared across fabric and fabric-ca:

- github.com/hyperledger/fabric/bccsp
- github.com/hyperledger/fabric/common/flogging
- github.com/hyperledger/fabric/common/metrics (including the gendoc utility)

The [PR](https://github.com/hyperledger/fabric-ca/pull/404) over in fabric-ca finally removes the fabric-ca dependency on core fabric.

This commit updates fabric to use the common code in fabric-lib-go.

For now a temporary branch in fabric-lib-go is used, see the corresponding [commit](https://github.com/hyperledger/fabric-lib-go/commit/cdae4d4a292dbad122b93a2c5c70bc61d846e990).
After this PR is reviewed and merged fabric-lib-go will be released and the dependency here will be updated to a real versioned release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 02:52:46 +0000 UTC
    </div>
</div>


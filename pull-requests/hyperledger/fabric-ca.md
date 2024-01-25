---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Bump mysql to mysql-apt-config_0.8.29-1_all.deb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump mysql to mysql-apt-config_0.8.29-1_all.deb.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 19:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Remove the Fabric 1.4 dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change is necessary to remove Fabric 1.4 dependencies in the CA.  The older dependencies are no longer maintained and a source of ongoing security exposures.  This change is the first of several to remove the the older dependencies.  This change refactors the CA to use Fabric 2.5.X dependencies.

This is a partial answer to the following:
https://github.com/hyperledger/fabric-ca/issues/376

This a refactoring effort with no new functionality.  Existing tests are sufficient.

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

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
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
        Created At 2024-01-18 19:06:21 +0000 UTC
    </div>
</div>


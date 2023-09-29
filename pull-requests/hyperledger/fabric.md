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
                PR <a href="https://github.com/hyperledger/fabric/pull/4451" class=".btn">#4451</a>
            </td>
            <td>
                <b>
                    Update pluggable_endorsement_and_validation.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #2814

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

Node SDK no longer supports chaincode deployment, and therefore the referenced doc page doesn't exist anymore. In this case the entire following sentence should be deleted.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

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
        Created At 2023-09-29 10:05:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4449" class=".btn">#4449</a>
            </td>
            <td>
                <b>
                    Clean up duplicated check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix duplicated check of file existence and clean up.

Change-Id: If162b6fbfebffd493f345439d346881068916b74

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset removes a duplicated check of the existence of the metadata file, and directly uses the err, which is common following Go style.

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
        Created At 2023-09-26 21:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4448" class=".btn">#4448</a>
            </td>
            <td>
                <b>
                    Fix typo in code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change the message of using commond --> command.

And minorly improve several comments.

Change-Id: I4321aa2b5b67aebd2be13ea8ce797c448cb86f6a

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Fix typo in the message and improve code comments.

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
        Created At 2023-09-25 23:02:57 +0000 UTC
    </div>
</div>


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
                PR <a href="https://github.com/hyperledger/fabric/pull/4933" class=".btn">#4933</a>
            </td>
            <td>
                <b>
                    chore: fix some comments
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

<!--- Describe your changes in detail, including motivation. -->

 fix some comments


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
        Created At 2024-07-28 17:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4932" class=".btn">#4932</a>
            </td>
            <td>
                <b>
                    Added a check to make sure that chaincode is actually running.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found that sometimes chaincode won't start. It waits for "Ready" message, but another message comes to it, for example "Init".
This happens when another transaction arrives during chaincode start. And it falls between the two events:
- Handler for chaincode is already there - the start process has started
- "Ready" state has not yet occurred.

I corrected the situation by checking the Handler state as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-24 22:02:44 +0000 UTC
    </div>
</div>


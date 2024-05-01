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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4829" class=".btn">#4829</a>
            </td>
            <td>
                <b>
                    orderer: fix function names
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


 fix function names

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
        Created At 2024-04-28 07:13:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4827" class=".btn">#4827</a>
            </td>
            <td>
                <b>
                    add mutex usage comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement

#### Description

This PR adds a comment describing the mutex `blockAPIsRWLock`.

#### Additional details

It was found out that removal of some `blockAPIsRWLock` read locks gives better performance for HLF peer and reduces its resource downtime. But after clarification for what this read locks had been made, the clarifying comment was added.

#### Related issues

Initial performance improvements and discussion are available in the [PR#4694](https://github.com/hyperledger/fabric/pull/4694).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 09:02:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4826" class=".btn">#4826</a>
            </td>
            <td>
                <b>
                    add unit test against a real grpc server for common/deliverclient/blo…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Test update

### Description
fix https://github.com/hyperledger/fabric/issues/4567

Update unit test for deliveryRequester.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 19:55:01 +0000 UTC
    </div>
</div>


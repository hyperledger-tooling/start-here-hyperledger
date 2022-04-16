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
                PR <a href="https://github.com/hyperledger/fabric/pull/3329" class=".btn">#3329</a>
            </td>
            <td>
                <b>
                    new caas page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature
- Documentation update

#### Description

New page for running chaincode as a service on the test network.

https://github.com/hyperledger/fabric-samples/blob/main/test-network/CHAINCODE_AS_A_SERVICE_TUTORIAL.md

https://hyperledger-fabric.readthedocs.io/en/latest/cc_service.html


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-16 01:05:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3325" class=".btn">#3325</a>
            </td>
            <td>
                <b>
                    Bump zap-logfmt
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

- Improvement (improvement to code, performance, etc)


#### Description

Update zap-logfmt from v0.0.2 to v0.0.4

<!--- Describe your changes in detail, including motivation. -->

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

- #3260 

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
        Created At 2022-04-10 00:12:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3324" class=".btn">#3324</a>
            </td>
            <td>
                <b>
                    Use actual address of the deadMembers2Expire slice variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Instead of passing the address of the for-loop variable, pass address of the 
actual slice element.

Signed-off-by: Artem Barger <artem@bargr.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 20:13:52 +0000 UTC
    </div>
</div>


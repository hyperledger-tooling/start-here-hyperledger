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
                PR <a href="https://github.com/hyperledger/fabric/pull/4312" class=".btn">#4312</a>
            </td>
            <td>
                <b>
                    feat(workflow): add workflow for checking broken links
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
- Add a Github Action to look for broken links on the latest version of the documentations / release notes
- This does NOT resolve the broken links, this PR adds a way to continuously check for them
<!--- Describe your changes in detail, including motivation. -->

#### Additional details
- Resolving the broken links are not handled within this PR to limit the scope of work
- Add a Github Action using the [muffet](https://github.com/raviqqe/muffet) library 
- Schedule the Github Action workflow to be everyday at 01:50 UTC 
- Set the option commands 

`--max-response-body-size=100000000` 
`--buffer-size=2147483647`
-> set extra body size to handle downloads links (ex. zip files)

`--rate-limit=10`
`--timeout=20`
-> resolves rate-limit / timeout error seen during the execution on Github action job 

`--color=always`
-> always enable all colored output during the execution on Github action job 

`--exclude="^(https:\/\/hyperledger-fabric.readthedocs.io\/[A-z_]+\/(v[\d]+.[\d]+.[\d]+|release)).*$" https://hyperledger-fabric.readthedocs.io/en/latest/`
-> Exclude any links that direct to the documentation or release notes of the non-latest version to limit the scanning to target to that of the latest version



<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues
**Partially**-solves https://github.com/hyperledger/fabric/issues/2814
The remaining scope is to resolve the broken links reported by this workflow.
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
        Created At 2023-07-09 03:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4310" class=".btn">#4310</a>
            </td>
            <td>
                <b>
                    docu:typo-fix-in-gateway.md
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

By referring the issues no #3271
fixes the typo mistake in "Have"--->> "Having"
fix issue #3271


#### Additional details

Step to resolved issue 
Go to website 
[clickhere](https://hyperledger-fabric.readthedocs.io/en/latest/gateway.html#)

Screenshot :- 
![image](https://github.com/hyperledger/fabric/assets/109129126/f01e0e56-6e1b-4e61-9597-d5fe8e296e9f)



Here  i am solved that issue #3271
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 05:58:19 +0000 UTC
    </div>
</div>


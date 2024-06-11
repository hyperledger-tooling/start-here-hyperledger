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
                PR <a href="https://github.com/hyperledger/fabric/pull/4891" class=".btn">#4891</a>
            </td>
            <td>
                <b>
                    Replace ioutil.WriteFile with os.WriteFile
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
This PR replaces the deprecated ioutil.WriteFile with os.WriteFile to comply with the latest Go standards and improve code maintainability.

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

<!--- Describe your changes in detail, including motivation. -->
The Go standard library package `ioutil` has been deprecated, and its functions have been moved to other packages. This change updates the code to replace `ioutil.WriteFile` with `os.WriteFile` in the `core/deliverservice/deliveryclient_test.go` and `common/deliverclient/blocksprovider/deliverer_test.go` files. This ensures that the code adheres to the latest Go standards and improves maintainability.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->
The changes were made in the test files and were tested by running the existing unit tests to ensure that the new `os.WriteFile` function works as expected without any issues.

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->
No related issues.

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
        Created At 2024-06-10 21:29:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4889" class=".btn">#4889</a>
            </td>
            <td>
                <b>
                    chore: make function comments match function names
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

make function comments match function names

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
        Created At 2024-06-09 11:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4888" class=".btn">#4888</a>
            </td>
            <td>
                <b>
                    Remove DCO github action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that the integrated DCO app is working again,
we don't need the extra DCO github action.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 18:00:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4887" class=".btn">#4887</a>
            </td>
            <td>
                <b>
                    Address review comments for Remove global endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address review comments for Remove global endpoints.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 17:27:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4886" class=".btn">#4886</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.22.4 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.22.4.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 15:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4885" class=".btn">#4885</a>
            </td>
            <td>
                <b>
                    Replace DCO bot with local action.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

Replace DCO bot with local check.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 13:27:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4884" class=".btn">#4884</a>
            </td>
            <td>
                <b>
                    up go 1.22.4
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
        Created At 2024-06-05 06:32:04 +0000 UTC
    </div>
</div>


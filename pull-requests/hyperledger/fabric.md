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
                PR <a href="https://github.com/hyperledger/fabric/pull/4895" class=".btn">#4895</a>
            </td>
            <td>
                <b>
                    bump github.com/stretchr/testify v1.9.0
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
        Created At 2024-06-16 07:01:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4893" class=".btn">#4893</a>
            </td>
            <td>
                <b>
                    bump github.com/golang/protobuf v1.5.4
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
        Created At 2024-06-15 13:05:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4892" class=".btn">#4892</a>
            </td>
            <td>
                <b>
                    Implement 'osnadmin channel info' subcommand and update tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Implemented the `osnadmin channel info` subcommand to retrieve detailed information about a specific channel from an Ordering Service Node (OSN). This involved modifying the CLI commands and adding corresponding functionality to interact with the channel participation API.

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

<!--- Describe your changes in detail, including motivation. -->
Implemented the `osnadmin channel info` subcommand to retrieve detailed information about a specific channel from an Ordering Service Node (OSN). 



<!--- Additional implementation details or comments to reviewers. -->
- Introduced `info` subcommand under `osnadmin channel` to support querying individual channel details.
- Updated existing tests and added new tests to cover the new feature and edge cases.


Closes #4890


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 18:37:30 +0000 UTC
    </div>
</div>

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


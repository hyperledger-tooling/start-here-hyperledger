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
                PR <a href="https://github.com/hyperledger/fabric/pull/3226" class=".btn">#3226</a>
            </td>
            <td>
                <b>
                    Add Intermediate CA certs to dial options (backport #3225)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3225 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 16:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3225" class=".btn">#3225</a>
            </td>
            <td>
                <b>
                    Add Intermediate CA certs to dial options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway was omitting to include TLS intermediate certificates in the dial options when connecting to other nodes.
This commit appends them to the splice of root certs in the endpoint config.

Resolves #3224 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 11:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3222" class=".btn">#3222</a>
            </td>
            <td>
                <b>
                    Filter out purged data from private data store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Description
This PR  introduces support for the purge marker(s) and filters the data marked for purging. In addition, this PR removes the 
unused code for V11 format as now we upgraded data format along with retroactively creating hashed index at peer start.

#### Related issues
Resolves #3028 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 14:07:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3221" class=".btn">#3221</a>
            </td>
            <td>
                <b>
                    Fix typo in orderer.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Muhammad Anas Baig <anasbaigmughal@gmail.com>

## Fix typo

#### Type of change

- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 18:10:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3219" class=".btn">#3219</a>
            </td>
            <td>
                <b>
                    Include chaincode tutorial in getting Getting Started section of docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also minor wording and link updates to content related to the client API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 14:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3218" class=".btn">#3218</a>
            </td>
            <td>
                <b>
                    ledgerutil exits with a proper code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch makes ledgerutil exit with a proper code when it fails.

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The ledgerutil command exits with 0 (success) whether or not it succeeds in the comparison; it exits with 1 (failure) only when the parsing of the command line arguments are unsuccessful.

This patch makes it exit with 1 additionally when
- it fails in the comparison of snapshots
- it finds that the snapshots are different after the comparison
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 08:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3215" class=".btn">#3215</a>
            </td>
            <td>
                <b>
                    Fix gossip unit test flake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increasing the timeout in the gossip service unit tests appears to reduce the occurence of the flake that we frequently observe.

This should be seen as a tactical fix while the underlying cause is investigated.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 14:52:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3214" class=".btn">#3214</a>
            </td>
            <td>
                <b>
                    Encode Hashed Data To Hexadecimal
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

- Bug fix
- Improvement (improvement to code, performance, etc)

#### Description

- Hashed data (snapshot record hashed keys and values) was not properly converting to string due to JSON encoding not supporting certain special characters, resulting in data loss. Hashed data is now converted to hexadecimal string to maintain data integrity.
- JSON output now contains new boolean field, hashed, indicating whether diffRecord has hashed data (key and value).

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


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
        Created At 2022-02-07 03:34:18 +0000 UTC
    </div>
</div>


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
                PR <a href="https://github.com/hyperledger/fabric/pull/4226" class=".btn">#4226</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.4 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.4 (release-2.2).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 20:07:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4225" class=".btn">#4225</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.4 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 20:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4224" class=".btn">#4224</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 20:05:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4222" class=".btn">#4222</a>
            </td>
            <td>
                <b>
                    Update event service documentation. (backport #4221)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4221 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 12:47:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4221" class=".btn">#4221</a>
            </td>
            <td>
                <b>
                    Update event service documentation.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove outdated information about the original v1.0 event hub.
- Provide summary of event service.
- Clarify block events versus chaincode events.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 22:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4217" class=".btn">#4217</a>
            </td>
            <td>
                <b>
                    Orderer v3: SmartBFT: eliminate Consnsus.Type in orderer.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Ieddc902e711de7a0f7dabc76111dde100abb185e

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: SmartBFT: eliminate Consnsus.Type in orderer.yaml

#### Related issues

#4216 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-14 15:29:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4214" class=".btn">#4214</a>
            </td>
            <td>
                <b>
                    Update chaincode_lifecycle.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Content updates - docs #3276
Changing from "new" to "v2.x"

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
        Created At 2023-05-10 13:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4213" class=".btn">#4213</a>
            </td>
            <td>
                <b>
                    Update references to system channel in swagger definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update references to system channel in swagger definition of channel participation API

#### Type of change

- Documentation update

#### Description

As described in issue #4194 .

#### Related issues

issue #4194 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 09:07:43 +0000 UTC
    </div>
</div>


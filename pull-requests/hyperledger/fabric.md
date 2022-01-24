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
                PR <a href="https://github.com/hyperledger/fabric/pull/3189" class=".btn">#3189</a>
            </td>
            <td>
                <b>
                    Address windows platform in documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #2993
Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

Address how windows users can install and contribute to fabric. The current documentation was inaccurate


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 17:20:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3188" class=".btn">#3188</a>
            </td>
            <td>
                <b>
                    remove redundant requirements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

This removes some redundant text from writing first app. You do not need windows build tools or any linux build tools for this tutorial but also this information about how to install build tools is out of date (ie not correct anymore) and in the case of linux, also specific to ubuntu (and may not work on other distros)

contributes to #2993 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 14:19:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3186" class=".btn">#3186</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.17.5 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.17.5.

First commit runs goimports to fix up build instructions.
Second commit updates unit tests and dependencies to work with Go 1.17.5.
Third commit updates docs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 05:02:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3183" class=".btn">#3183</a>
            </td>
            <td>
                <b>
                    Wire-in retroactive creation of hashed-index in pvtdatastore at peer start
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
This PR adds code for invoking the function for creating hashed-indexes in pvtdatastore at the time of peer start.

#### Related issues
issue# 3022

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 15:54:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3182" class=".btn">#3182</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.17.5 (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.17.5 (release-2.4)

Backport 3 commits from main branch related to Go 1.17 update, including dependency updates and test fixes.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 20:15:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3178" class=".btn">#3178</a>
            </td>
            <td>
                <b>
                    Refactor gateway Endorse() method (backport #3171)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3171 done by [Mergify](https://mergify.com).


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
        Created At 2022-01-18 22:48:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3177" class=".btn">#3177</a>
            </td>
            <td>
                <b>
                    typo in word 'oreder'.Changed to 'order'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update

#### Description
There was a typo in word 'oreder'. Changed it to 'order'.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 08:28:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3176" class=".btn">#3176</a>
            </td>
            <td>
                <b>
                    Close connections to stale ordering nodes (backport #3172)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3172 done by [Mergify](https://mergify.com).


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
        Created At 2022-01-18 04:42:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3175" class=".btn">#3175</a>
            </td>
            <td>
                <b>
                    Fixing some typos
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

<!--- Describe your changes in detail, including motivation. -->
Fixing some typos.

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
        Created At 2022-01-17 18:45:09 +0000 UTC
    </div>
</div>


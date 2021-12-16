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
                PR <a href="https://github.com/hyperledger/fabric/pull/3128" class=".btn">#3128</a>
            </td>
            <td>
                <b>
                    Update 'Running a Fabric Application' tutorial for Fabric Gateway (backport #3110)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3110 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-16 13:02:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3127" class=".btn">#3127</a>
            </td>
            <td>
                <b>
                    Reduce CPU&memory cost of collecting endorsements (backport #3119)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3119 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-15 14:04:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3126" class=".btn">#3126</a>
            </td>
            <td>
                <b>
                    Enable gateway concurrency limits (backport #3123)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3123 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-15 14:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3123" class=".btn">#3123</a>
            </td>
            <td>
                <b>
                    Enable gateway concurrency limits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for setting API invocation concurrency limits on the gateway service.  Uses the same mechanism as used by the endorser and deliver services.

The sample config limit has been set to 500 for now.  This can be adjusted in the future based on experience.

Resolves https://github.com/hyperledger/fabric-gateway/issues/344

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 10:52:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3121" class=".btn">#3121</a>
            </td>
            <td>
                <b>
                    fix typo in docker-env.mk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Wang Zhuo <zhuowangy2k@outlook.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

This change fixes two typos in the docker-env.mk.

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
        Created At 2021-12-14 17:04:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3119" class=".btn">#3119</a>
            </td>
            <td>
                <b>
                    Reduce CPU&memory cost of collecting endorsements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Based on performance analysis of the gateway, the following changes are made in this commit:
1. Instead of collecting and holding copies of all proposal responses in order to reuse the protoutil.CreateTx() function, just store a single response payload and all of the signed endorsement objects.  Check that all payloads are bitwise idential and endorsers are unique at collection time.
2. Eliminate the duplicate unmarshalling that was occurring as a result of reusing protoutil.CreateTx

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 11:47:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3118" class=".btn">#3118</a>
            </td>
            <td>
                <b>
                    Remove discovery.acl principal warning (backport #3116)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3116 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-13 12:50:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3116" class=".btn">#3116</a>
            </td>
            <td>
                <b>
                    Remove discovery.acl principal warning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #3006 added warnings for principal check failures to assist with troubleshooting.
The discovery warning was too much however since even in normal scenarios
discovery endorser service checks the peer against the various channel principals.
This change reverts to the prior code without the warning.

Resolves https://github.com/hyperledger/fabric-gateway/issues/349.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 06:36:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3115" class=".btn">#3115</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.17.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.17.5.
Fix unit tests to work with Go 1.17.5.
Update dependencies to work with Go 1.17.

Resolves #3073 

Signed-off-by: David Enyeart enyeart@us.ibm.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-12 20:40:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3114" class=".btn">#3114</a>
            </td>
            <td>
                <b>
                    Go 1.17 prep - ignore vendor directory in staticcheck
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A few vendored dependencies have benign staticcheck errors
when using Go 1.17.

This commit simply filters out vendor directories in staticcheck output
since the intention of the linter is to check Fabric source only.

Note - it is not possible to filter the vendor directories as input to staticcheck,
as they will still show up when the Fabric package that uses them gets checked.
Have to filter the output instead.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 16:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3113" class=".btn">#3113</a>
            </td>
            <td>
                <b>
                    updating peer-chaincode-devmode.md (backport #3099)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #3099 done by [Mergify](https://mergify.com).


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
        Created At 2021-12-10 19:11:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3111" class=".btn">#3111</a>
            </td>
            <td>
                <b>
                    Update the Makefile target for release/
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updating the release/xxx target to include the cc builders in the tgz
The dist/xxx target was originally updated, but the actual publishing from the fabric-interop test doesn't use this target.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 09:55:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3110" class=".btn">#3110</a>
            </td>
            <td>
                <b>
                    Update 'Running a Fabric Application' tutorial for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also fixed a few build warnings in other documents.

Contributes to #2807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 22:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3109" class=".btn">#3109</a>
            </td>
            <td>
                <b>
                    Update config transaction validation logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix misleading debug message.
Log info when channel config is applied.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 21:59:26 +0000 UTC
    </div>
</div>


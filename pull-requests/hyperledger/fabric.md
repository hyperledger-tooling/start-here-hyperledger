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
                PR <a href="https://github.com/hyperledger/fabric/pull/3132" class=".btn">#3132</a>
            </td>
            <td>
                <b>
                    - Fix failure to generate all possible combinations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

Bug happens when the endorsement policy is set to k-out-of-n where (n - k) > 1.
For example, when there are 6 organizations and the endorsement policy is set
to majority (i.e. 4-out-of-6). The combinations calculated by chooseKoutOfN()
in original code are as below.
	[0 1 2 5], [0 1 2 5], [0 1 2 5], [0 1 3 5],
	[0 1 3 5], [0 1 4 5], [0 2 3 5], [0 2 3 5],
	[0 2 4 5], [0 3 4 5], [1 2 3 5], [1 2 3 5],
	[1 2 4 5], [1 3 4 5], [2 3 4 5]

Obviously, the function fails to find out all the possible combinations. Some of
 the combinations are overrided by child's call. This bug would trigger below
error sometimes when the alive peers are not within the above combinations.

	[discovery] chaincodeQuery -> ERRO 13a Failed constructing descriptor for
	chaincode chaincodes:<name:"XXXX" > ,: no peer combination can satisfy the
	endorsement policy

To fix it, the last line of choose() should be changed to pass a copy of
"currentSubGroup" to the recursive call instead, i.e.

	choose(n, targetAmount, i+1, append(make([]int, 0), currentSubGroup...), subGroups)

After applying the fix, the resulting combinations generated should be corrected
as below.
	[0 1 2 3], [0 1 2 4], [0 1 2 5], [0 1 3 4],
	[0 1 3 5], [0 1 4 5], [0 2 3 4], [0 2 3 5],
	[0 2 4 5], [0 3 4 5], [1 2 3 4], [1 2 3 5],
	[1 2 4 5], [1 3 4 5], [2 3 4 5]

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 09:20:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3131" class=".btn">#3131</a>
            </td>
            <td>
                <b>
                    v2.4.1 release commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update release notes, documentation, and scripts for v2.4.1.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 19:42:33 +0000 UTC
    </div>
</div>

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


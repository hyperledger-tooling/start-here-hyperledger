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
                PR <a href="https://github.com/hyperledger/fabric/pull/3493" class=".btn">#3493</a>
            </td>
            <td>
                <b>
                    Update secured-private-asset-tranfer documentation and tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: fraVlaca <ocsenarf@outlook.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:47:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3492" class=".btn">#3492</a>
            </td>
            <td>
                <b>
                    Fix regex in install-fabric script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Running `./install-farbic.sh` or `./install-fabric.sh samples binary docker` should clone the samples, download the binaries, and download docker images, but it only clones the samples. The regex only took the first argument, so they are changed to take all arguments.

Signed-off-by: Youngeon Lee <youngl@bu.edu>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-18 13:54:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3490" class=".btn">#3490</a>
            </td>
            <td>
                <b>
                    Updates in main for release v2.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates docs and scripts in main for latest release v2.4.4.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 17:27:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3489" class=".btn">#3489</a>
            </td>
            <td>
                <b>
                    test: use `T.TempDir` to create temporary test directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

A testing cleanup. 

This pull request replaces `ioutil.TempDir` with `t.TempDir`. We can use the `T.TempDir` function from the `testing` package to create temporary directory. The directory created by `T.TempDir` is automatically removed when the test and all its subtests complete. 

This saves us at least 2 lines (error check, and cleanup) on every instance, or in some cases adds cleanup that we forgot.

Reference: https://pkg.go.dev/testing#T.TempDir

```go
func TestFoo(t *testing.T) {
	// before
	tmpDir, err := ioutil.TempDir("", "")
	require.NoError(t, err)
	defer os.RemoveAll(tmpDir)

	// now
	tmpDir := t.TempDir()
}
```

#### Additional details


#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 17:03:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3488" class=".btn">#3488</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update release notes, documentation, and scripts for v2.2.6.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 14:07:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3487" class=".btn">#3487</a>
            </td>
            <td>
                <b>
                    Release commit for v2.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update release notes, documentation, and scripts for v2.4.4.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 13:49:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3486" class=".btn">#3486</a>
            </td>
            <td>
                <b>
                    [WIP] Add purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work in progress to add private data purge integration tests

#### Type of change

- Test update

#### Related issues

[Private data purge RFC](https://github.com/hyperledger/fabric-rfcs/blob/main/text/0000-private_data_purge.md)

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 16:43:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3485" class=".btn">#3485</a>
            </td>
            <td>
                <b>
                    Fix gossip unit test flake (backport #3215)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3215 done by [Mergify](https://mergify.com).


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
        Created At 2022-06-16 14:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3484" class=".btn">#3484</a>
            </td>
            <td>
                <b>
                    Fix gossip unit test flake (backport #3215)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3215 done by [Mergify](https://mergify.com).


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
        Created At 2022-06-16 14:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3483" class=".btn">#3483</a>
            </td>
            <td>
                <b>
                    Add logging for identity, policy, and signature troubleshooting (2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport #3006

Most identity, policy, and signature issues return a fairly generic error
message to the user, e.g. "not authorized".
This is often intentional so as to not disclose information to malicious users that
may be probing for information about the system.

This commit adds logging on the orderer and peer side so that identity issues
can more easily be troubleshooted by users setting up sample networks,
and by administrators and SREs in production networks.

For any identity, policy, or signature error, the failed policy and passed identity is now logged in a warning message.
Additionally, the identity of every signature that is verified can be seen if tracing is enabled.

The new logging can help with the following types of issue resolution:
User cert and MSP membership errors
Determine which user is unauthorized to perform an action
Determine which MSPs and user signatures are included in a config transaction that was invalidated
Determine which peers participated in an endorsement invalidation
Determine which peer signature doesn't match the others in a proposal response

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 12:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3481" class=".btn">#3481</a>
            </td>
            <td>
                <b>
                    Update Ledgerutil Docs
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

- Update the documentation for the ledgerutil tool suite by updating the compare command docs and adding identifytxs docs

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

#3466 

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
        Created At 2022-06-15 21:57:33 +0000 UTC
    </div>
</div>


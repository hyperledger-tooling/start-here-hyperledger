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
                PR <a href="https://github.com/hyperledger/fabric/pull/3502" class=".btn">#3502</a>
            </td>
            <td>
                <b>
                    Add OpenTelemetry interceptors to capture traces from gRPC communications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #2954 - was closed for inactivity while #2997 was pending.

#### Type of change
- New feature

#### Description

Adds OpenTelemetry tracing by adding interceptors on all gRPC communications.

#### Related issues
This is tied to https://github.com/hyperledger/fabric-rfcs/blob/main/text/0000-opentelemetry-tracing.md

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 21:31:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3500" class=".btn">#3500</a>
            </td>
            <td>
                <b>
                    Check if inner consensus message is missing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An orderer to orderer consensus message that contains an empty inner message crashes the node because it attempts to figure out its type and the mere action of determining the type of a nil pointer, causes a panic.

This commit ensures the inner message is not nil.

Change-Id: I06b466e6ff6d43f2b9804dd21185241716356050
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 15:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3498" class=".btn">#3498</a>
            </td>
            <td>
                <b>
                    upgrade to Ginkgo v2
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
- Test update

#### Description

<!--- Describe your changes in detail, including motivation. -->
upgrade ginkgo to v2

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
        Created At 2022-06-21 11:43:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3495" class=".btn">#3495</a>
            </td>
            <td>
                <b>
                    Check if inner consensus message is missing (backport #3494)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3494 done by [Mergify](https://mergify.com).


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
        Created At 2022-06-21 08:23:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3494" class=".btn">#3494</a>
            </td>
            <td>
                <b>
                    Check if inner consensus message is missing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An orderer to orderer consensus message that contains an empty inner message crashes the node because it attempts to figure out its type and the mere action of determining the type of a nil pointer, causes a panic. 

This commit ensures the inner message is not nil. 

Change-Id: I06b466e6ff6d43f2b9804dd21185241716356050
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 20:58:01 +0000 UTC
    </div>
</div>

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


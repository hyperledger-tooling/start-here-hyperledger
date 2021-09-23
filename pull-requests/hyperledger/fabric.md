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
                PR <a href="https://github.com/hyperledger/fabric/pull/2942" class=".btn">#2942</a>
            </td>
            <td>
                <b>
                    Unit test flake when rpc server stream not closed (backport #2935)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 21:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2940" class=".btn">#2940</a>
            </td>
            <td>
                <b>
                    Unit test flake when rpc server stream not closed (backport #2935)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2935 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 21:46:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2939" class=".btn">#2939</a>
            </td>
            <td>
                <b>
                    Fixed Found Typos
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

- Fixed found typos throughout fabric code

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
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
        Created At 2021-09-21 16:24:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2936" class=".btn">#2936</a>
            </td>
            <td>
                <b>
                    FAB-2931: do not create a chain if it's already created (backport #2934)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2934 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 19:19:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2935" class=".btn">#2935</a>
            </td>
            <td>
                <b>
                    Unit test flake when rpc server stream not closed
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
This Unit test fails randomly in more recent PR builds(https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40922&view=logs&j=e306c17a-d139-54bf-a475-f5a11259cee7&t=1e3023a5-584f-52f3-49bc-66bd27d27b6d, https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40557&view=logs&j=6b58850f-3858-5a05-33e2-5e41cbf03c4e&t=bddec1cf-ba37-5883-9c3e-fd1e8608f9a1, https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40922&view=logs&j=e306c17a-d139-54bf-a475-f5a11259cee7&t=1e3023a5-584f-52f3-49bc-66bd27d27b6d)

Testcase: 
orderer/common/cluster_test.TestSendSubmitWithReport

Analysis/Observation: 
Problem 1: Testcase expects to fail at SubmitRequest after node server restarts with error EOF, but if restart not closed the streams before sendSubmit submitted; test fails. It is random failure. This PR introduces a delay between restart and submitRequest.

Problem 2: Calling t.FailNow() from other than main test go-routine, won't terminate all other subroutines. (which is called in this testcase from require.EqualError(t, err, io.EOF.Error())) This is the reason for the testcase hangs/blocked. https://pkg.go.dev/testing#B.FailNow.  Updated the testcase to signal & terminate the testcase from test main go-routine.

#### Related issues
#2835 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 12:57:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2934" class=".btn">#2934</a>
            </td>
            <td>
                <b>
                    FAB-2931: do not create a chain if it's already created
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Vladyslav Kopaihorodskyi <vlad.kopaygorodsky@gmail.com>

#### Type of change
- Bug fix


#### Description

Do not create a new chain of type `etcdraft.Chain` if such exists in the map of chains. This can happen when in Raft protocol a channel was created, but not marked as done in WAL logs. So at orderer startup, it tried to create another instance of a chain and panicked because that instance startup failed. 

#### Related issues

#2931 


#### Release Note
Fixed bug when an orderer crashed at channel creation and after restart couldn't bootstrap because of desynchronization between WAL logs and ledger state.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-18 00:58:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2933" class=".btn">#2933</a>
            </td>
            <td>
                <b>
                    Apply the style only the key in readwrite.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the style from '``k5,``' to '``k5``',

Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change
- Documentation update

#### Description
Apply the style only the key in readwrite.rst

Fix the style from '```k5,```' to '```k5```,' in 

> T5 passes validation because it reads a key, k5, which was not modified by any of the preceding transactions

in [Read-Write set semantics](https://hyperledger-fabric.readthedocs.io/en/latest/readwrite.html)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 14:26:23 +0000 UTC
    </div>
</div>


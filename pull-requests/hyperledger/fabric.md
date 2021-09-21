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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2927" class=".btn">#2927</a>
            </td>
            <td>
                <b>
                    Cache channel orderers in registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently discovery is invoked to get the list of channel orderers on each Submit() request (the orderer connections are cached).
This enhancement caches the list of orderers and registers a callback with the channel config update bundle to trigger cache refresh

resolves #2911 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 11:20:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2926" class=".btn">#2926</a>
            </td>
            <td>
                <b>
                    Fix broken links for international workgroups (#2920) (backport #2921)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span><span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2921 done by [Mergify](https://mergify.io).


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
        Created At 2021-09-16 11:15:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2925" class=".btn">#2925</a>
            </td>
            <td>
                <b>
                    Fix broken links for international workgroups (#2920) (backport #2921)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span><span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2921 done by [Mergify](https://mergify.io).


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
        Created At 2021-09-16 11:15:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2924" class=".btn">#2924</a>
            </td>
            <td>
                <b>
                    Fix the result message in test_network.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the result message on running "./network.sh createChannel"

The result message format has been changed from the change of
test-network/scripts/createChannel.sh in hyperledger/fabric-samples
since
b690d8f Stop using deprecated outputAnchorPeersUpdate in test-network (#394)

#### Type of change
- Documentation update

#### Description
Fix the result message on running ```./network.sh createChannel```

The result message format has been changed from the change of
test-network/scripts/createChannel.sh in hyperledger/fabric-samples
since
[b690d8f Stop using deprecated outputAnchorPeersUpdate in test-network (#394)](https://github.com/hyperledger/fabric-samples/commit/b690d8f30f0e47f9512bc2620e95a413f54f6039#diff-848fb64f9085c01d8a264cf33696747f639a7bd6c7d48eb95e35ba1ffd5e7f70L64)

I've run the fabric-samples and have gotten the below log.
```
Channel 'mychannel' joined
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 09:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2921" class=".btn">#2921</a>
            </td>
            <td>
                <b>
                    Fix broken links for international workgroups (#2920)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The list of international workgroups was moved
from https://wiki.hyperledger.org/display/fabric/International+groups
to https://wiki.hyperledger.org/display/I18N/International+groups.

Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change

- Documentation update

#### Description
Broken links have been used in the documentation.

#### Additional details
The list of international workgroups was moved
from https://wiki.hyperledger.org/display/fabric/International+groups
to https://wiki.hyperledger.org/display/I18N/International+groups.
But the documentation has used the old one.

#### Related issues
#2920 (https://github.com/hyperledger/fabric/issues/2920)

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 06:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2919" class=".btn">#2919</a>
            </td>
            <td>
                <b>
                    Update docs for Jira to GitHub issue transition (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs to indicate that GitHub issues are now
used instead of Jira issues.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 16:24:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2918" class=".btn">#2918</a>
            </td>
            <td>
                <b>
                    Update docs for Jira to GitHub issue transition (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs to indicate that GitHub issues are now
used instead of Jira issues.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 16:18:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2909" class=".btn">#2909</a>
            </td>
            <td>
                <b>
                    Write config blocks synchronously in Orderer
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
Assume the config block contains a transaction which removes the
node from consenters, the consensus chain will switch to follower
chain which reads last config block from ledger directly. Because of
writing config block asynchronously, follower chain maybe read a
stale config block in which the node is still a consenter. So the
node will switch back to a consenter again.

Writting config blocks synchronously would fix this bug.

#### Related issues
Resolves #<2908>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 08:45:12 +0000 UTC
    </div>
</div>


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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2907" class=".btn">#2907</a>
            </td>
            <td>
                <b>
                    Update docs for Jira to GitHub issue transition
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
        Created At 2021-09-13 22:00:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2905" class=".btn">#2905</a>
            </td>
            <td>
                <b>
                    Updates in main for v2.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and scripts in main branch for v2.3.3 release.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:40:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2903" class=".btn">#2903</a>
            </td>
            <td>
                <b>
                    Release commit for v2.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.3.3.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 18:58:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2901" class=".btn">#2901</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.2.4.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 18:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2900" class=".btn">#2900</a>
            </td>
            <td>
                <b>
                    updated chaincode4ade.rst("Writing your first chaincode") showing good practise on how to achieve determinism in json
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
        Created At 2021-09-08 15:00:23 +0000 UTC
    </div>
</div>


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
                PR <a href="https://github.com/hyperledger/fabric/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    Improve error message for a non-existent block delivery failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Improve error message when delivery service is asked for a block that doesn't yet exist on the node to make it more clear for users or support personnel.

#### Related issues
Fixes https://github.com/hyperledger/fabric/issues/3320


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 13:46:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3338" class=".btn">#3338</a>
            </td>
            <td>
                <b>
                    Updated dockerfile with new build arg
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

Added a new arg to pass in machine architecture details

#### Related issues

#3337 


Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 13:17:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3335" class=".btn">#3335</a>
            </td>
            <td>
                <b>
                    Handle empty policies when traversing the policy tree in discovery policy analysis (backport #3334)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3334 done by [Mergify](https://mergify.com).


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
        Created At 2022-04-18 10:17:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3334" class=".btn">#3334</a>
            </td>
            <td>
                <b>
                    Handle empty policies when traversing the policy tree in discovery policy analysis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Discovery policy analysis engine assumed that the inner policy passed to it is of the correct type and cannot be empty.
Added a nil check and a test.

Change-Id: Ia6eaf0211d8d9f4b7f2881547934dc32c725a458
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 08:31:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3329" class=".btn">#3329</a>
            </td>
            <td>
                <b>
                    new caas page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature
- Documentation update

#### Description

New page for running chaincode as a service on the test network.

https://github.com/hyperledger/fabric-samples/blob/main/test-network/CHAINCODE_AS_A_SERVICE_TUTORIAL.md

https://hyperledger-fabric.readthedocs.io/en/latest/cc_service.html


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-16 01:05:05 +0000 UTC
    </div>
</div>


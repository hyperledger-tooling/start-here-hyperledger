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
                PR <a href="https://github.com/hyperledger/fabric/pull/4434" class=".btn">#4434</a>
            </td>
            <td>
                <b>
                    add docs for smartbft metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 18:13:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4433" class=".btn">#4433</a>
            </td>
            <td>
                <b>
                    Document chaincode upgrade impact on state data (backport #4432)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4432 done by [Mergify](https://mergify.com).


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
        Created At 2023-09-07 15:31:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4432" class=".btn">#4432</a>
            </td>
            <td>
                <b>
                    Document chaincode upgrade impact on state data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document chaincode upgrade impact on state data.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 13:51:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4431" class=".btn">#4431</a>
            </td>
            <td>
                <b>
                    Bft bp deliveryclient censorshiptimeout 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code)
- Test update

#### Description

As described in issue #4401 

#### Related issues

issue #4401 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 09:28:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4430" class=".btn">#4430</a>
            </td>
            <td>
                <b>
                    smart BFT GRPC broadcasting invalid TX to leader test
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

Test that invalid TX broadcast to the leader is failing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:48:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4429" class=".btn">#4429</a>
            </td>
            <td>
                <b>
                    Smart BFT GRPC forwarding invalid message test
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

A test to check that if an orderer is forwarding to the leader an invalid TX, the operation should fail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:45:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4426" class=".btn">#4426</a>
            </td>
            <td>
                <b>
                    Update bootstrap script for v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update old bootstrap.sh script to match the newer install-fabric.sh script.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 13:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4424" class=".btn">#4424</a>
            </td>
            <td>
                <b>
                    Fix install-fabric.sh to pull baseos for v3.x
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

Fixed install-fabric.sh to pull baseos images for v3.x as well as v2.x.

#### Additional details

#### Related issues

https://github.com/hyperledger/fabric/issues/4423
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 01:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4422" class=".btn">#4422</a>
            </td>
            <td>
                <b>
                    up consensus library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-03 21:44:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4421" class=".btn">#4421</a>
            </td>
            <td>
                <b>
                    Add v3.* tags as a trigger to release job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add v3.* tags as a trigger to release job.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 11:28:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4419" class=".btn">#4419</a>
            </td>
            <td>
                <b>
                    Release notes v3.0.0-preview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release notes for v3.0.0-preview release.

Also delete old v2.5.x release notes that are now maintained in release-2.5 branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 02:08:43 +0000 UTC
    </div>
</div>

